# PostgreSQL Database Dump

This repository contains a dump of a PostgreSQL database, showcasing its structure using a table named `queries`. The dump includes the schema and an empty table ready for data insertion.

## Table of Contents

- [Schema](#schema)
- [Import Instructions](#import-instructions)
- [License](#license)

## Schema

The database schema consists of a single table, `queries`, with the following columns:

- `id` (integer)
- `username` (character varying, max length 50)
- `querydate` (timestamp without time zone, default: CURRENT_TIMESTAMP)
- `type` (character varying, max length 10)
- `document` (character varying, max length 18)
- `referreddate` (date)
- `interval` (character varying, max length 10)
- `interval_label` (character varying, max length 10)

## Import Instructions

To use this database dump:

1. Clone this repository:

    ```bash
    git clone https://github.com/yourusername/your-repository.git
    ```

2. Import the database dump into your PostgreSQL database:

    ```bash
    psql -U your_username -d your_database -f path/to/database_dump.sql
    ```

   Make sure to adjust the connection details accordingly.

3. Start querying or insert your own data into the `queries` table.

## License

This database dump is provided under the [MIT License](LICENSE). Feel free to use, modify, and distribute it as needed.
