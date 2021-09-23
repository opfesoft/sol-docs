# holiday\_dates

## Structure

| Field            | Type    | Attribute | Key | Null | Default | Extra | Comment |
|:-----------------|---------|-----------|-----|------|---------|-------|---------|
| id               | int     | unsigned  | PRI | NO   |         |       |         |
| date_id          | tinyint | unsigned  | PRI | NO   |         |       |         |
| date_value       | int     | unsigned  |     | NO   |         |       |         |
| holiday_duration | int     | unsigned  |     | NO   | 0       |       |         |

## Description of fields

### id

Holiday ID from [Holidays DBC file](../../dbc/Holidays.md).

### date_id

ID of the date, increased by 1 for every year.

### date_value

The start time of the holiday in a packed format. To get the actual dates this query can be used:

```sql
SELECT *,(`date_value` >> 24) & 0x1F AS `year`, ((`date_value` >> 20) & 0xF) + 1 AS `month`, ((`date_value` >> 14) & 0x3F) + 1 AS `day`, (`date_value` >> 6) & 0x1F AS `hour`, `date_value` & 0x3F AS `minute` FROM `holiday_dates`;
```

To create a packed date use this function:
```sql
CREATE FUNCTION `packDate` (`year` TINYINT UNSIGNED, `month` TINYINT UNSIGNED, `day` TINYINT UNSIGNED, `hour` TINYINT UNSIGNED, `minute` TINYINT UNSIGNED)
RETURNS INT UNSIGNED DETERMINISTIC
RETURN (`year` << 24) | ((`month` - 1) << 20) | ((`day` - 1) << 14) | (`hour` << 6) | `minute`;
```

Examples:
```sql
SET @PACK_DATE := packDate(21,7,14,12,30);
SELECT @PACK_DATE;
```

```sql
INSERT INTO `holiday_dates` (`id`, `date_id`, `holiday_duration`, `date_value`)
VALUES
(999,0,0,packDate(21,7,14,12,30));
```

### holiday_duration

The number of hours of how long the holiday may last (visible in the calendar).
