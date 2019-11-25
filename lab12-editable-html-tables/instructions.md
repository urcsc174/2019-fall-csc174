# Lab 12: Editable HTML Tables

*Due: Monday, November 25, 2019 (today)*

The purpose of this lab assignment is to quickly find and implement a solution to enable the ability to read and write to a MySQL table using an *editable* HTML form.

## Requirements

Using your localhost, install a solution that has all four "C.R.U.D." capabilities that work within a single HTML table without refreshing the webpage:

- [ ] (Create) Ability to **add** new records to the table using an HTML form *in* the table
- [ ] (Read) Pulls data from a MySQL table and **displays** it in an HTML table
- [ ] (Update) Ability to **edit/update** existing records in the table, "inline"
- [ ] (Delete) Ability to **delete** records from the table, selectively

## Hints

- Search Google for a solution, and peruse the tutorials for one that looks well-written and easy to implement. 
  - When using Google, include the names of the language(s) you want the solution to use
  - Find a good one that works? Post a link to it in our **Slack #chatter** channel; when verified, the professor will ***exempt* you from your current lowest lab grade**
  - Beware of solutions that use PHP **mysql_** commands instead of mysql**i**_ (...with the **i**)
  - Beware of solutions that do not include an ADD (create) function - check out the demo if available
  - If frustrated, try this one but be aware: it doesn't used a standard "connection" file.  If you use it, you should fix that!
    - [https://www.webslesson.info/2017/07/live-add-edit-delete-datatables-records-using-php-ajax.html](https://www.webslesson.info/2017/07/live-add-edit-delete-datatables-records-using-php-ajax.html)
    - Using this solution will not qualify you for the *lowest lab grade exemption*
  - Here is another solution that works, however it doesn't edit "in-line" rather it uses modal dialog boxes (overlays) over the table to allow editing.
    - [https://www.phpflow.com/php/addedit-delete-record-using-bootgrid-php-mysql/](https://www.phpflow.com/php/addedit-delete-record-using-bootgrid-php-mysql/)
    - NOTE: "Bootgrid" is someone's customized version of Bootstrap with some extra features
    - Using this solution will not qualify you for the *lowest lab grade exemption*

## Install the Application

When you got the application working correctly on your localhost, install it on the class web server.

#### Setup Your Data Table on the Class Web Server

- [ ] Export your local database table to an export file (typically called **export.sql**); then edit the table name in the SQL code to use your first initial, last name (e.g. **rkostin_data** ...note: instead of "_data" you should use whatever makes sense for your application)

- Login to our class **Bluehost** account and make your way over to the **phpMyAdmin** application
- Click the **urcscon3_lab12**
- [ ] **Import your exported SQL** to create your data table

#### Edit the Application's Database Connection Information

- [ ] Edit your **configuration file** to work with a database (already created) on the class web server

```sql
'localhost'
'urcscon3_lab12'
'[same password ...you know what it is]'
'urcscon3_lab12'
```

*...NOTE: the database server (the host) is still "localhost"*


#### FTP Your Files to the Class Web Server

- Note: as always, everyone will be using the same FTP account in this class so be careful when you're working on the web server!  Be careful *not* to disturb other students' files.

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: lab12@csc174.org
FTP Password: [same as before]
```

*Notice that the username is always different*

- [ ] FTP your files into a folder using your first initial, last name (e.g. **rkostin**)

## Test the Application

Then open a web browser pointed to your application on the class web server: 

​	**csc174.org/lab12/**

If everything works, you're good to go.  (No need to submit anything in Blackboard.)  The professor will check your handiwork on the class web server late in the day on the due date and give you credit (pass/fail)
