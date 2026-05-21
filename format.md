# Data Format Instructions

## Regions
For this field, use the decimal form of a binary number.
This number should be up to 4 bits.
Each bit should be a 1 if the game is for that region, and a 0 if it isn't.

**In order from least significant (rightmost) bit to most significant (leftmost) bit:**
- Europe
- North America
- Japan
- Other

### Most Common Region Values
Use the decimal values in the CSV file.
| Game Region(s) | Binary | Decimal |
| --- | --- | --- |
| North America | 0010 | 2 |
| Europe | 0001 | 1 |
| Japan | 0100 | 4 |
| NA + Japan | 0110 | 5 |
| NA + Europe | 0011 | 3 |
| World | 1111 | 15 |
| Not China/Korea | 0111 | 7 |

## Save Type
Here's a reference chart with the different save type values used in the database:
| Value | Save Type |
| --- | --- |
| 0 | 8K EEPROM |
| 1 | 8K EEPROM (256M ROM) |
| 2 | 64K EEPROM |
| 3 | 64K EEPROM (256M ROM) |
| 8 | 512K FLASH (with RTC) |
| 9 | 512K FLASH |
| 10 | 1M FLASH (with RTC) |
| 11 | 1M FLASH |
| 14 | 256K SRAM |
| 15 | None (No Saving) |

## Multi-Line Titles
This is for programs that display the game title in up to 2 lines (some just use 1), similar to the DS/DSi and 3DS menus (including TWLMenu++).
The columns "Title Line 1" and "Title Line 2" are for these titles. Not all games will use the "Title Line 2" column; for these games, just leave it blank.
