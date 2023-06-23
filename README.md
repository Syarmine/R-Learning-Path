## R-Learning-Path
Documenting my R Learning Journey from Dataquest


### Working with Data Sources using SQL (SQLite)
The types of operations SQL can perform are often referred to as CRUD, or "create, read, update, delete". Most databases consist of multiple tables of data. Like a table in a spreadsheet, a database table consists of rows and columns which are often called records (rows) and fields (columns). 

Each table in a database may be connected to other tables through fields that relate to one another. This type of database is called a relational database, A database can store large amounts of data more securely and efficiently than a spreadsheet or a text file. However, unlike simply opening a spreadsheet, we need to "ask" for data from the database. This is what we do when we write queries in SQL.

| Command | Description|
| ------- | ---------- |
| `SELECT`| selection |
| `*` | special character meaning 'all' |
|  , | to reduce number of field shown from `SELECT`, use comma as separator | 
| ; | to end the syntax |
| `FROM` | where to read data from |
| `LIMIT` | returns the number of rows returned |
| `AS` | will let you temporarily rename or alias these fields, Aliasing fields does not permanently change their name in the database. Aliases only exist for as long as the query does.  |
| `--` or `/* */` | -- for single line comments, /* */ for multiline comments |

### Exploring Tables and Columns

For consistency and efficiency, SQL databases only allow one type of data per column. This means that integer columns only have integers, text columns only have text, and so on. Formally, these types of data storage classes. Even though datatypes and storage classes are different, it's common to refer to both of them as datatypes.

SQLite terminology:
| Terminology | Definition |
| ------- | -------|
| _Integer_ | integer numbers, like the values in the quantity field |
| _Real_ | for floats or decimal numbers |
| _Text_ or string | for text or strings data types. There is no storage class for date, the db stores date as texts |  

| Command | Description|
| ------- | ---------- |
| `PRAGMA table_info()`|  retrieves metadata, which is information about a table. |
| `Column A * X` | Operating on Numeric Columns for a calculated field |

### Sources

- [Dataquest](https://app.dataquest.io/)
- [SQLite](https://www.sqlite.org/pragma.html#pragma_table_info:~:text=PRAGMA%20schema.table_info(table%2Dname)%3B)
