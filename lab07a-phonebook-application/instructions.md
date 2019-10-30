# Lab 7a: Phonebook Application

*Due: Monday, October 28, 2019 (today)* 

In this exercise you will extend the database and table you setup last time to include more information.

At the end of this lab, you'll have a set of working website files on your localhost.  Hold on to them because in our next class we'll do, Lab 7**b** (the second part), which will involve you installing the same working website on the class web server.

*Note: if you don't have a local database with a "phonelist" table, download [the files from last time (ZIP)](../15-php-mysql2/four-functions.zip) and catch-up*

## Edit the Existing Table

Start your localhost (MAMP or WAMP) and open **phpMyAdmin**

- [ ] In your database from Lab 6 (**demo1**?) click on the table we added (**phonelist**?)
- [ ] Looking at the *structure* of the phonelist table, find the area that says Add "1" column(s) "after..."
  - Change the "1" to "2" columns
  - Click the **Go** button
- [ ] Setup the two new columns:
  - Name: **phone**, Type **VARCHAR**, Length/Values **50**
  - Name: **email**, Type **VARCHAR**, Length/Values **100**
  - Click the **Save** button

You can close or put-aside phpMyAdmin for now

## Edit the Application to Work with the New Table Columns

- [ ] Go to your web root and find the files from last class.  Also, open your web browser and go to **localhost**.  Make sure you still can connect to the database with your *phonelist* table - use the **testmysql.php** to confirm

If your localhost is working correctly and you've confirmed you can connect to your database, use your web browser to navigate to the phonebook application (the files from last class).

Notice in the phonebook application that there are only two fields being shown (besides ID): First Name and Last Name ...but the table you created in the database has *two more fields*: **phone** and **email**.  The bulk of this lab is to hack the code you've been given to work with the fields.  

*Note: for some CSC 174 students (especially those with no prior programming experience) this might be tricky, but not impossible! Carefully look at the lines of code indicated in the instructions below and make the changes as needed to get the application to work with the two new database fields.*

- [ ] Edit **renderform.php**

  - edit **line 3**; insert two new variables *between* `$lastname` and `$error`: <br>**\$phone** and **\$email**<br>...and be careful with the commas!

  - duplicate **lines 21** and **22** (create new lines 23 and 24) and edit the duplicates to make them work with the new variables **\$phone** and **\$email**

- [ ] Edit **index.php**
  - duplicate **lines 19** and **20** and edit the duplicates as needed
  - duplicate **lines 31** and **32** and edit the duplicates as needed

- [ ] Edit **new.php**:
  
  - duplicate and edit **lines 10** and **11**
  - edit **line 16**
  - edit **line 20**
  - edit **line 25** (be very careful with this one; very difficult with all the quotes and commas)
- edit line **32** (add two more empty quotes with commas)
  
- [ ] Edit **edit.php**
  - duplicate and edit **lines 13** and **14**
  - edit **line 19** (be careful with the double-pipes ...means OR)
  - edit **line 24**
  - edit **line 28** (be very careful with this one; very difficult with all the quotes and commas)
  - duplicate and edit **lines 49** and **50**
  - edit **line 55**

- [ ] Then test all four functions in your web browser
  - If all four database functions continue to work then just leave your files and database as-is until next time when we'll move them to the class web server
  - If any of the four functions don't work you'll need to figure out where you went wrong and fix it before the next class



