# IMPLEMENTATION-OF-DDL-COMMANDS-TO-CREATE-A-LTER-AND-DROP-TABLE

AIM:

To execute SQL commands for creating tables, altering and dropping the table from a
database.

PROCEDURE:

1. ALTER command
alter command is used for altering the table structure, such as,

1. to add a column to existing table

2. to rename any existing column

3. to change datatype of any column or to modify its size.

4. to drop a column from the table.

ALTER Command: Add a new Column

Using ALTER command, we can add a column to any existing table.

Syntax:

ALTER TABLE table_name ADD(column_name datatype);

Example:

ALTER TABLE

ALTER Command: Add multiple new Columns

Using ALTER command we can even add multiple new columns to any
existing table.

Syntax:

ALTER TABLE table_name ADD( column_name1 datatype1,column-name2 datatype2, );

ALTER Command: Add Column with default value

ALTER command can add a new column to an existing table with a default value too.
The default value is used when no value is inserted in the column.

Syntax:

ALTER TABLE table_name ADD( column-name1 datatype1 DEFAULT some_value);

ALTER Command: Modify an existing Column

ALTER command can also be used to modify data type of any existing column.

Syntax:

ALTER TABLE table_name modify( column_name datatype);

ALTER Command: Rename a Column

Using ALTER command you can rename an existing column.

Syntax:

ALTER TABLE table_name RENAME COLUMN old_column_name TO new_column_name;

ALTER Command: Drop a Column

ALTER command can also be used to drop or remove columns.

Syntax:

ALTER TABLE table_name DROP column (column_name);

2..TRUNCATE command
TRUNCATE command removes all the records from a table. But this command will not destroy the table's structure. When we use TRUNCATE command on a table its (auto-
increment) primary key is also initialized.

Syntax:

TRUNCATE TABLE table_name;

Example:

TRUNCATE TABLE EMPLOYEE;

3.DROP command

DROP command completely removes a table from the database. This command will also destroy the table structure and the data stored in it.
Syntax:

DROP TABLE table_name;

Example:

DROP TABLE EMPLOYEE;

COMMANDS:

SQL> ALTER TABLE CUSTOMERS ADD SEX char(1);

SQL>SELECT * FORM CUSTOMERS;

SQL> ALTER TABLE CUSTOMERS DROP SEX;

SQL>SELECT * FORM CUSTOMERS;

SQL> TRUNCATE TABLE CUSTOMERS;

SQL>SELECT * FORM CUSTOMERS;

Empty set (0.00 sec)

SQL> DROP TABLE CUSTOMERS;

Query OK, 0 rows affected (0.01 sec)

SQL> DESC CUSTOMERS;

ERROR 1146 (42S02): Table 'TEST.CUSTOMERS' doesn't exist
