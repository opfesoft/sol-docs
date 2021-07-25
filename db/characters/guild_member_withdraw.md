# guild\_member\_withdraw

This table is used to track the limited daily withdrawals for the guild bank.

## Structure

| Field           | Type    | Attributes | Null | Key | Default | Extra | Comment |
|-----------------|---------|------------|------|-----|---------|-------|---------|
| [guid](#guid)   | int(10) | unsigned   | NO   | PRI | NULL    |       |         |
| [tab0](#tab0-5) | int(10) | unsigned   | NO   |     | 0       |       |         |
| [tab1](#tab0-5) | int(10) | unsigned   | NO   |     | 0       |       |         |
| [tab2](#tab0-5) | int(10) | unsigned   | NO   |     | 0       |       |         |
| [tab3](#tab0-5) | int(10) | unsigned   | NO   |     | 0       |       |         |
| [tab4](#tab0-5) | int(10) | unsigned   | NO   |     | 0       |       |         |
| [tab5](#tab0-5) | int(10) | unsigned   | NO   |     | 0       |       |         |
| [money](#money) | int(10) | unsigned   | NO   |     | 0       |       |         |

## Description of the fields

### guid

The player's GUID. See [characters.guid](characters.md#guid)

### tab0-5

The amount of item withdrawals for the affected tab ID. See [guild\_bank\_tab.TabId](guild_bank_tab.md#tabid)

### money

The amount of money withdrawn.
