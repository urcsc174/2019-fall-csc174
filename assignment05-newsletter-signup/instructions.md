# Assignment 5: Newsletter Signup

*Due: Monday, November 11, 2019 (one week)* 

The goal of this assignment is to take your midterm project and power it with PHP so it writes to a MySQL database.

*NOTE: this assignment is different - instead of being a team effort, everyone must work individually and turn-in their own website.  You will be graded on your ability to perform all three developer roles: IA, Designer, and Technician.*

## Requirements

NOTE: although you are using your Midterm Project for this assignment, you will not be graded on the particulars of the midterm except where specified in the instructions below.  I.e., there will be a different rubric.

NOTE: there is *no* requirement for a **readme.md** file for this assignment. 

### Architecture

- [ ] The website must be restructured to support these goals:
  - Set the **primary goal**  of the website to getting users to *sign-up for the newsletter*
  - The **secondary goal** of the website is to get users to read more about the website's topic, and *then* sign-up for the newsletter
- [ ] Part of the new architecture includes what happens *after* the user fills out the form and submits it  (there must be some confirmation of what the user did after the form is submitted)
  - EXTRA CREDIT: if you can figure out how to get the "thank you" to replace the HTML form after it's sucessfully submitted without going to a new webpage, you'll get a bonus 10 points (100 points max) ...hint: google a solution; also use the word **ajax** as part of your search term

Note: you can alter or add to the content in the website as needed to  support the new, primary goal

###### Architecture Grading

- [ ] Your architecture will be graded on the correct implementation of the goals (above) as well as...
- [ ] Semantically correct naming of files and folders, and semantic usage of *all* HTML tags
  - Example: do not use the P tag for anything but a true "paragraph"
- [ ] In addition to the document outline, i.e. the headings, all content must structured correctly, i.e. be positioned (nested) in the correct structural elements (main, section, article, et cetera).
  - Example: do not use the ARTICLE tag for anything but a true "article"
  - Also remember to use a DIV *only* as the tag of last resort! 

### Design

For the most part you can simply continue using the CSS as-is from your original Midterm Project, but improvements can be made at this point.

- [ ] You will continue to be graded on your understanding and implementation of the **C.R.A.P. principles**, **page layout**, and **typography** in terms of readability and legibility; remember, design must support the content ...not arbitrarily picked 
- [ ] You must continue to correctly implement the **Gutenberg rule** on all webpages (assuming an audience of left-to-right readers)
- [ ] You must continue to use a **CSS Architecture** that is easily understood and obvious. 

###### Design Grading

- [ ] The design must support the overall choreography from the homepage, to the HTML form, to the "thank you" content in a way that is clear and obvious; a design that creates *friction* (reduces click-through) will lose points
- [ ] The style and design of the **HTML form** - how it's positioned and how it integrates with the style of the overall website; using plain, unstyled form elements will lose points
  - NOTE: use of BR tags will lose points!  Use semantically correct HTML and CSS to layout your HTML form
- [ ] You will be graded on the style and design of the **post-form presentation** (what does the user see after the user clicks submit?)

### Technical Standards and Best Practices

- [ ] You must create a dedicated table and database to capture input from the website's HTML form
- [ ] You must add the appropriate PHP code to the website to write the form data to the table in the database

Note: out of the four database functions (**Create**, **Read**, **Update**, and **Delete** ...known as "CRUD" ) you need to implement the **create** function only for this assignment.  

###### Technical Grading

In addition to powering the website's HTML form to work with a MySQL database, you are still responsible for the usual technical requirements:

- [ ] All HTML and CSS must **validate within reason**; all PHP must work **without error**
  - On the class web server, PHP errors will automatically generate a `error_log` file to help you debug your PHP mistakes.  Be sure to **delete any error log files off the server** before your assignment is graded
- [ ] File naming conventions and file sizes must follow **industry standards**
- [ ] Demonstrate your ability to use **PHP Includes** to factor out a reasonable amount of common-code across the webpages

You are responsible for the correct installation of the website on the class web server, both files and database

- [ ] The website **files** must be installed on the BLUEHOST class web server using the following FTP login credentials

  - NOTE: everyone will use the same FTP account. Be careful *not* to disturb other students' files.

  ```
  FTP Server (a.k.a. Hostname): ftp.csc174.org
  FTP Port: 21
  FTP Username: assignment05@csc174.org
  FTP Password: [same as before - ask if you need to be reminded]
  ```
  
  - In this area, create a folder based on your first initial and last name, e.g. **rkostin** and put your assignment 5 files in there.  

- [ ] The website must use a **table** that you create in an existing database setup in our class' BLUEHOST account

  - You'll need to login to the class' hosting account on BLUEHOST.  

  ```
  www.bluehost.com
  username: csc174.org
  password: [same as the FTP password]
  ```
  
  - Then navigate into the **cpanel** and then to **phpMyAdmin**

- [ ] Using *phpMyAdmin* in Bluehost, create a **table** with a name styled like this:<br>`flastname_newsletter` <br> ...using your first initial and last name, e.g. **rkostin_newletter**

- [ ] Then build the table using fields and data types that correspond with the data captured from your HTML form

NOTE: everyone will use the same database; be careful *not* to disturb other students' tables in the database.

- [ ] Your PHP connect file will need to use the following connection information

  ```
  Hostname: localhost
  Username: urcscon3_assign5
  Password: [same as the FTP password]
  Database: urcscon3_assign05
  ```

  *Notice that the username and database name are not exactly the same!* (That's a Bluehost particularity)

## Submit the Assignment

- Make a submission in Blackboard, in the assignment: **Assignment 5: Newsletter Signup** and provide a link to your website on the class web server

