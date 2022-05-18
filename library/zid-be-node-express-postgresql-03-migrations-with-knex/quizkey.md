## Node, Express, and Postgres: Migrations with Knex

1. What is a database migration?

    **Answer:** A. A change to the structure of the tables

2. What actions require a database migration?

    **Answers:** A and C.

    A. Adding a secondary address field to the _suppliers_ table

    C. Renaming the _providers_ table to _suppliers_

3. What are the benefits of having a Knex migration file defined?

    **Answers:** A, B, and D.

    A. Easily sharing database configurations with other team members

    B. Having a single source of truth for the database schema across all environments

    D. Being able to undo database changes with rollback features

4. Which of the following are true about timestamps?

    **Answers:** A, B, C, and D.

    A. The `table.timestamps(true, true)` method will add *created_at* and *updated_at* columns.

    B. Timestamps are important because they help keep track of the table's records.

    C. Timestamps are not only used for logging purposes, they may also add functionality to an application.

    D. It's a best practice to use timestamps.
