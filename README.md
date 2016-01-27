## Task

You must implement required features in a Ruby on Rails application. This application will be responsible for reading log data from a file, storing it into a database, passing data to an external application via shell commands and displaying results on a web interface. 

Any changes made to the Ruby on Rails project must be done via Pull Requests. If there are any comments, they must be addressed before merging. You may merge once a :+1: is received. 

## Component 1: Log Parsing

The application must parse a log file. This file is named `log.txt` in the root of this project. 

## Component 2: Database Storage

Each field from the log file should be parsed and stored in the database. Along with the log data, each row should at least have an `id`, and the time at which the entry was inserted into the database. 

## Component 3: Shell Out

If an entry has an executable extension (.pdf or .exe) the `shasum` of the file must be sent to an external script `sha_lookup` and the result stored in the database.

## Component 4: User Interface
The web interface should display the log data from the database. 

* By default, it should be ordered by file name and date in a descending format. 
* The time should be displayed in a user-friendly format. 
* The user should have the ability to remove rows from being displayed. 
* The user should be able to search the file path.
* The order should be customizable via a GET request. 
 