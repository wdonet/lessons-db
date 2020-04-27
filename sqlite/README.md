# SQLite3
It's a binary DB built and use by C++ apps.

## Installation
Go to [downloads](https://www.sqlite.org/download.html) and pick the one for your OS

## Create DBs
If database does not exist, it creates a new one.
`sqlite3 [name].db`

## Common commands
- `.databases` - show databases
- `.tables` - show tables
- `.excel` - then executes any query and the outputs is exported as an CSV file

More [here](https://www.sqlite.org/cli.html)

## Run SQL statements
At the prompt `sqlite>` just write sql statements ending with a semicolon (`;`). If no semicolon and hits enter key, it will use next line to continue the current command definition.

### Results
They come in `list` mode by default which shows values separated by a pipe char (|).  That can be change by separator command, i.e. `.separator ","`.

There are mor modes for displaying results
- `.mode quote` - output is formatted as SQL literals. 'String\'s', blobs in hexadecimal, numbers as ASCII text and null as 'NULL'.
- `.mode line` - each column ion a line in the format `columnName = value`
- `.mode column` - data align by columns like in mysql CLI
- `.mode insert` - make the output looks like a set of insert sql statements
- `.mode insert` - shows the output in a HTML table (using TR and TD tags)

## Help
All input lines starting with a dot "." will be intrepreted as commans.  For getting help on those commands execute `.help` or `.help [command]` for more especific help at the command.
