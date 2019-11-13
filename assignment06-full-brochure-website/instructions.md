# Assignment 6: Full Brochure Website

*Due: Wednesday, November 20, 2019 (one week)* 

**The goal** of this assignment is to build a "brochure-type" website that also uses the best practices we've learned so far in CSC 174, plus all the best practices and standards from CSC 170.  

- [ ] Use [our team list (Google Sheet)](https://docs.google.com/spreadsheets/d/1vkAjS8dGcFF_ByS9VRuI8sGagDNTyrp8JF43sN_mf4M/edit#gid=0) to establish your role in a new city-team (due today, November 13)
- [ ] Each team must report ([in the Google Sheet](https://docs.google.com/spreadsheets/d/1vkAjS8dGcFF_ByS9VRuI8sGagDNTyrp8JF43sN_mf4M/edit#gid=0)) the topic of their brochure website (due tomorrow, November 14)

Remember: you have to **complete each role (IA, Designer, Technician) at least once** during the semester. This is a **team assignment**, however you will be graded for the work you do as an individual within the team.  

## General Requirements

The team is responsible for delivering a website that meets the following requirements:

- [ ] **Primary goal**: an informational website on a specific topic
- [ ] **Secondary goal:** the website must contain some "Contact Us " functionality that allows the user to fill-out an HTML form to request someone to contact them
- [ ] **Other requirement:** a back-end, mySQL database to capture the user input from the HTML form
  - Note: of the four database functions ("C.R.U.D"), this assignment requires CREATE only, i.e. create a record in the database
- [ ] **Other requirement:** the designer is required to use a **CSS Framework**.

### Information Architect's Requirements

The IA must deliver basic "content and intent" by **Friday (by end-of-day or so)** and then continue to add/update content up to the final due date for the assignment

Note: after the IA considers themself done with the content, the Designer and Technician may change the tags used in the HTML documents while they work. Keep in mind, the IA will be graded for the HTML structure in the *final* delivery.  So the IA must watch how the other team members add or change their HTML documents!  *If the designer and/or technician make mistakes in the HTML, the IA will lose points for it*

Also note: **the topic**, decided by the team, can have content from an existing website.  If so, consider this assignment a re-design of that website, where you have to make significant improvements to get a good grade.  (Simply replicating the existing website will lose points.)

- [ ] By <u>Friday</u>, the **content** must be represented in a set of **initial documents, structured in HTML**.  Although it does not have to be complete at this point - it can contain placeholder text and images - there must be enough structure and content for the Designer and Technician to begin work.
- [ ] At the end of the assignment, the IA will be graded on: everything described above plus...
  - The quality of the content: enough, written-well, suitable for use in a common "brochure-like" website
  - The semantic naming of files and folders, and semantic usage of the HTML tags
  - In addition to the first-level tags that surround content (e.g. P tags, H tags, et cetera), all content must be positioned (nested) in structural elements (e.g. main, section, article, et cetera)
- [ ] In addition, the **domain & ontology** of the website, a consistent **taxonomy**, and a clear and sensible **choreography** must be self-evident in the website
  - BTW, no **readme.md** file required for this assignment, however it's advisable to use one in your team's repository for team communication - but it will not be graded

### Design Artist's Requirements

The Designer's due date is the same as the due date for the overall website: **next Wednesday**:

- [ ] The designer must select a **CSS Framework** to use and then use it for a substantial amount of the website's visual design
- [ ] Design choices must support the *intent* of the content, i.e. no arbitrary choices - colors, imagery, behaviors, and typography must make sense in the context of the content
- [ ] The designer *must* extend the styles of the CSS Framework by writing and using **custom CSS** in their own CSS files (never altering the framework's files), and if necessary, adding a **override.css** file.

### Technician's Requirements

The Technician's due date is the same as the due date for the overall website: **next Wednesday**:

- [ ] The website must follow industry best practices and standards which includes:
  - The file structure and files used for the website
  - HTML and CSS validation (within reason)
  - File sizes and feasibility of the code to run quickly and reliably in modern web browsers
  - Use of PHP includes to factor out common elements (if it makes sense to use them)
- [ ] The website must be installed on the BLUEHOST class web server in a folder with a name based on the team city that you're in. 

### Database Credentials

Each team will use the same MySQL database on the Bluehost web server.  

```
Remote host: 66.147.242.186
Local host: localhost

Database user: urcscon3_assign6
Database password: [same as all the other passwords]
Database name: urcscon3_assign6
```

Remember - it's counter-intuitive:

-  When working with your website on your localhost and using the remote database on the production web server, the host is "**66.147.242.186**"
-  When the website is installed on the production web server, the host is "**localhost**"

### Web Server Credentials

Each team will use the same FTP account. Be careful *not* to disturb other teams' files.

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: assignment06@csc174.org
FTP Password: [same as all the other passwords]
```

## Submit the Assignment

Note: even though you worked as a team, everyone will be graded as an individual based on the work you did. To get credit for your work:

- Everyone on the team must make a submission in Blackboard, in the assignment:<br> **Assignment 6: Full Brochure Website with Database**

- In the submission you must provide the following information:

  - **Your city-team name**
  - A list of **everyone's name** in your team (including your own) **and their role** (IA, designer, or technician)
  - A link to the **website**
  - A link to the **repository**

  *NOTE: <u>do not</u> write this information (above) in the comments section in Blackboard.  Use the "Write Submission" area*

