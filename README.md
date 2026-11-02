# ZunkerBot

A PHP-based bot project by [ItsWocky](https://github.com/ItsWocky).

## Contents

- `Config/` — Configuration files directory
- `zu/` — Core bot files/modules
- `zu.php` — Main PHP entry point / source file
- `zunker.sql` — Database schema/setup SQL file
- `zunker.sql~` — Database backup file
- `readme.txt` — Original text readme

## Requirements

- PHP installed and configured on your system
- A SQL database server (e.g., MySQL or MariaDB)

## Setup

1. Clone the repo or download it as a ZIP from the green **Code** button.
2. Set up your database by importing the `zunker.sql` file.
3. Configure your database credentials and bot settings inside the `Config/` folder.
4. Run the bot using the PHP entry point: `php zu.php`

## Configuration

- Database connection settings and other bot parameters are handled within the `Config/` folder.
- Ensure your database matches the schema provided in `zunker.sql`.

## Usage

- Run the script via your command line or host it on a PHP-enabled web server.
- Check the `Config/` folder and `readme.txt` for specific runtime instructions.

## Notes

- The presence of a backup SQL file (`zunker.sql~`) suggests the database is still actively being modified.

## Author

ItsWocky — [GitHub profile](https://github.com/ItsWocky)
ItsWocky — [GitHub profile](https://github.com/ItsWocky)

