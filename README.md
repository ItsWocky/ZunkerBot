# ZunkerBot

A PHP-based bot project by [ItsWocky](https://github.com/ItsWocky), distributed as a prebuilt Windows package.

## Contents

- `Config/` — Configuration files directory
- `zu/` — Core bot files/modules
- `zu.php` — Main PHP entry point / source file
- `zunker.sql` — Database schema/setup SQL file
- `zunker.sql~` — Database backup file
- `readme.txt` — Original text readme

## Requirements

- Windows (the build ships as a `.7z` archive)
- 7-Zip (or any archiver that handles `.7z`) to extract the package
- PHP installed and configured on your system
- A SQL database server (e.g., MySQL or MariaDB)

## Setup

1. Clone the repo or download it as a ZIP from the green **Code** button.
2. Extract `ZunkerBot.7z` into a folder of your choice.
3. Set up your database by importing the `zunker.sql` file.
4. Configure your database credentials and bot settings inside the `Config/` folder.
5. Run the bot using the PHP entry point: `php zu.php`

## Configuration

- Database connection settings and other bot parameters are handled within the `Config/` folder.
- Ensure your database matches the schema provided in `zunker.sql`.

## Usage

- Run the script via your command line or host it on a PHP-enabled web server.
- Check the `Config/` folder and `readme.txt` for specific runtime instructions.

## Notes

- The source is distributed inside a `.7z` archive; there is no browsable source tree in the repository.
- The presence of a backup SQL file (`zunker.sql~`) suggests the database is still actively being modified.

## Author

ItsWocky — [GitHub profile](https://github.com/ItsWocky)
