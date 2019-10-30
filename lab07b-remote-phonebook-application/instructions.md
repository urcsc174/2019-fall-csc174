# Lab 7b: Remote Phonebook Application

*Due: Wednesday, October 30, 2019 (today)*

In this exercise, for Part 1: you will take the database you created from Lab 7a (last time) and install it on the class web server; and you will alter your connection script to use the remote database from your localhost.

For Part 2: you will install your Phonebook Application files on the class web server and once again, alter the connection script as needed so the application continues to work while it's on the class web server.  

## Part 1: Localhost Files and Remote Database

Note: this part assumes you've successfully extended the table **phonelist** in a localhost database so it has five fields:

- id (int with auto incrementer)
- firstname (varchar 50)
- lastname (varchar 100)
- phone (varchar 50) <-- new!
- email (varchar 100) <-- new!

...and the PHP Phonebook Application files have been sucessfully altered to accomdate the new fields.

### Step 1: Export Your Database Table

- [ ] **Export** your table (not the database) from your local phpMyAdmin to an SQL file
- [ ] Open the SQL file for editing and **search and replace** all instances of `phonelist` with a prefix that uses your first initial and last name like this: `rkostin_phonelist`
  - In Sublime Text, highlight the text "phonelist" and press **control-command-G** (mac) or **alt-F3** (pc), then type the new name
  - You will find 8 occurances of "phonelist" in your export SQL file

Save and close the file and put it aside. You'll need it soon.

### Step 2: Login to Bluehost

- [ ] Go to www.bluehost.com

- [ ] Login with domain: **csc174.org**<br>And password: **[ask the professor]**
  - NOTE: please try and get the login right.  If you screw it up multiple times in a row, we'll all get locked out!

- [ ] Once logged-in, click **cpanel** in the submenu

Then put this web browser tab with your connection to Bluehost aside.  You'll need it later.

### Step 3a: Test Your Connection to the Remote Database

- [ ] Open your file: **testmysql.php** file in your localhost and change the login information to these new login settings.  

```php
$mysqli = new mysqli('66.147.242.186', 'urcscon3_lab07', 'coffee1N', 'urcscon3_lab07');
```

Notice the new login information: the IP number instead of "localhost" and the name of the database ...it's awkwardly long, but that's what Bluehost decided it must be

- [ ] Save the file and then open it in a web browser (using localhost).
  - Maybe you'll get the "Connection OK" message in the viewport because someone else in CSC 174 already registered your "Class C" with Bluehost; if so, skip the next step
  - Or, if after a long wait you get the "Connect Error (2002)" message, do the following step to setup remote access...

### Step 3b: Setup Remote Access to the Remote Database

You can skip this step if you got the "Connection OK" message in the previous step.  Else do the following.

- [ ] Go back to the web browser tab open to Bluehost
- [ ] In the cpanel, scroll down to click the **Remote MySQL** chicklet (or you'll probably find a link to it along the left-side, under "frequently used features")
- [ ] On the "Remote Mysql Database Access" page, click the [Add] link to add **Your Class C** (<u>not</u> *your IP*)
- [ ] When your Class C is showing in the text box, click the green **Add** button
- [ ] Go back to your web browser pointed at **testmysql.php** and refresh it;  you should get the "Connection OK" message in the viewport
- [ ] In the web browser tab pointed to Bluehost, click **cpanel** in the submenu to go back to the cpanel

### Step 4. Import the Database on the Remote Server

1. In the cpanel, scroll down to click the **phpMyAdmin** chicklet (or you'll probably find a link to it along the left-side, under "frequently used features")
2. In the left-side bar, click the name of our Lab 7 database, **urcscon3_lab07**
3. Click the **Import** tab in the top area
4. Click the **Choose File** button and select your edited SQL file from Step 1.
5. Scroll down and click the **Go** button

Hopefully, you'll see a long list of green messages.  If so, proceed to the next step.

### Step 5: Change the Connection Information

Go to your files for the Phonebook Applicaiton in your web root and find your **connect-db.php** and **connect-db REMOTE.php** files

- [ ] Rename **connect-db.php** to **connect-db LOCAL.php**
- [ ] Rename **connect-db REMOTE.php** to **connect-db.php**

Open the (newly renamed) **connect-db.php** file in your code editor and take a look at the login information; notice it's the new, remote login information from Step 3a.

### Step 6: Use the Remote Database with your Local Web Application

1. Open the following PHP files from the Four Functions web application in your code editor
   - **index.php**
   - **new.php**
   - **delete.php**
   - **edit.php**
2. Search for every instance of "**phonelist**" in those PHP files and replace them with the new table name based on your first initial and last name, example "**rkostin_phonelist**"
   - In **index.php** there is one instance
   - In **new.php** there is one instance
   - In **delete.php** there is one instance
   - In **edit.php** there are two instances
3. Save and close those files
4. Test the Phonebook Application  in your localhost again
   - Make some additions, edits, deletions ...whatever
   - In the phpMyAdmin that's pointed to the Bluehost web server (*not* your localhost) "browse" your table on the remote server; you should see your additions, edits, and deletions there

## Part 2: Remote Files and Remote Database

For this part you need to FTP your Phonebook Application to the class web server and make sure it continues to work.

- [ ] IMPORTANT: edit your **connect-db.php** file again. Change the `$server` information from `66.147.242.186` back to `localhost`

- [ ] Open your FTP software and login using the following web server credentials, below.<br>*Note: everyone will use the same FTP account. Be careful not to disturb anyone elses' files.*

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: lab07@csc174.org
FTP Password: [ask the prof]
```

- [ ] When you FTP-in to the account, create a folder using your first inital and last name (e.g. **rkostin** place your application files in there

Test the remote version of your remote application on the class web server: 

`csc174.org/lab07/flastname/`

## Turn It In

- [ ] When the remote application and database is working, login to our CSC 174 area in Blackboard and go into the "Labs and Assignments Turn-in" area
  - Find the assignment: **Lab 07: Phonebook Application**
  - Copy and paste the URL of your application into "Write Submission" 
  - Submit the assignment







NOTE: getting credit for this lab is automatic.  When the professor sees your table in the **urcscon3_lab07** database, he'll give you credit for this assignment in Blackboard.