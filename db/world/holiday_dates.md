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

The start time of the holiday.

### holiday_duration

The number of hours of how long the holiday may last (visible in the calendar).
