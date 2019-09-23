# Assignment 3: Information Architecture
*Due: Monday, September 30, 2019 (one week)*

The goal of this assignment is to build another team website based on other students' content and make it better.  

- The **IA** must make the website better by **imposing a proper information architecture** over the content (note: this is the most important part of this assignment)
- The **Designer** must make the website better by making visual *improvements* to the formatting and layout of the website
- The **Coder** must maintain or fix the quality of the website in terms of the file structure, optimization, and validation

## Requirements

### DUE: TODAY, Monday, September 23

1. **Everyone**: go to [our shared Google Sheet](https://docs.google.com/spreadsheets/d/1vkAjS8dGcFF_ByS9VRuI8sGagDNTyrp8JF43sN_mf4M/edit#gid=0) to choose a new team and a new role  
   - Everyone must chose a different role in a different city (COPY your name/email to a new column)
   - Note: you do not have to move as a group; suggestion - move to a ROLE you want to take-on next
   - Setup a *new* private team channel in Slack
2. After the team comes together, the **Coder** must create and setup a new repository, and the add the other team members as collaborators; the Coder must also make sure the rest of the team is able to sync the repo to their localhosts using the GitHub Desktop software
3. When the new repo is established and everyone in the team is setup as collaborators, the **Coder** needs to copy and paste a link to the repo in [our shared Google Sheet](https://docs.google.com/spreadsheets/d/1vkAjS8dGcFF_ByS9VRuI8sGagDNTyrp8JF43sN_mf4M/edit#gid=0) 

### DUE: by end-of-day Wednesday, September 25

*Note: this is the trickiest, most important part of this assignment.*

1. Working alone (typically) the **Information Architect** must search across all the student web pages from Assignment 2 and pick out the content from individual students (not entire three-student websites - just individual students and their four pages) 
   - All the student content picked must *not* be any of the students on your team
   - You can FTP into the assignment02 folder using the FTP instructions from Assignment 2, or better yet...
   - "Scrape" the content from the pages: http://csc174.org/assignment02/ so you can start building the document structure and outline from scratch (because undoubtedly, the other IA screwed it up)

MOST IMPORTANT: The **IA** needs to carefully select the students to find a *common thread* among the three - something you can build an *information architecture* around.

The goal of the **IA** is to *impose* an ontology, taxonomy and choreography on to the content.  That may mean getting/changing content including getting new images, altering or writing new headlines ...whatever it takes to FORCE the content into a proper information architecture.

Also note, the **IA** does not need to use ALL the content from the other students' webpages.  You can throw-out content that doesn't fit the new information architecture.  

1. The **IA** must setup the HTML pages and structure the content into a coherent document outline using semantically correct HTML tags
   - Note: it can be rough at first, but good enough for the Designer and Coder to have something to work with; remember, the content can be tweaked all the way until the assignment is turned-in next Monday
   - Also note: you do *not* have to create four pages for each student!!!  How you divide the content - long pages vs. separate pages, is up to you as the IA
2. The **IA** must create a **readme.md** file in the repository that clearly explains: 
   - The **domain** (a simple line or two of text that describes the subject matter; think "introduction"; make sure to explain what the three things that the students have in common)
   - The **ontology** (a list of *triples* that describes all the content in the website)
   - The **taxonomy** (which will typically translate into headings in the HTML)
   - The **choreography** (which will typically translate into the order and/or navigation)
3. The **IA** must sync the initial content and readme to the team's repository no later than **end-of-day on Wednesday, September 25**
   - NOTE: the **IA** does not have to finish the HTML by the due date - there only needs to be enough struture for the Designer and Coder to begin their work
   - IMPORTANT: if the **IA** has *not* made adequate progress with the HTML by Thursday morning, the professor will re-assign the job of IA to another student on your team
   - HINT: the **IA** should focus on building HTML in .html files - and they don't even have to be fully fleshed-out or valid HTML!  Leave the PHP Includes and the validation to the **Coder** for later.  
   - HINT: the **IA** does need to think about the navigation element(s); but does not have to think about where they get positioned or how they get styled!  Leave the styling (which includes positioning) to the **Designer** for later.

### By the assignment due date: Monday, September 30...

- [ ] The **Designer** must base their design off one of the existing styles from any of the Assignment 2 websites, and then make visual improvements
  - The **Designer** must leave a comment in thier main CSS file (typically styles.css) and indicate from which Assignment 2 they based their design (paste a URL to the Assignment 2 website)
  - The designer will be graded by IMPROVEMENTS to the basic readability and clarity of the typography
  - NOTE: the designer must pick and choose from <u>any</u> pre-existing Assignment 2 CSS to get "inspiration" - not necessarily the CSS from which any of the content came. However, keep in mind: the Designer will be graded on subjective *improvements* to the CSS.  Simply installing it as-is will be graded poorly.
- [ ] The **Coder** must ensure the new website meets all web standards and best practices, including but not limited to:
  - PHP Includes factor out redundant code (within reason)
  - The current page highlighter(s) works
  - All HTML and CSS meet W3C standards (within reason)
  - The source code (HTML, CSS, JavaScript and/or PHP) is properly formatted with whitespace and readable
  - The website is mounted on the class webserver and works correctly
    - Only files that are part of the website exist on the web server (e.g. no **readme.md** on the server!)
    - All file and folder names follow industry standards (all lowercase and no spaces)
    - File sizes (especially image files) are appropriate for the web

## Installation

- [ ] The **Coder** must install the website on the class web server using the following web server credentials, below.

Note: each team will use the same FTP account. Be careful *not* to disturb other teams' files.

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: assignment03@csc174.org
FTP Password: [same as before]
```

- [ ] **Coder**: when you FTP-in to the account, create a folder using the name of your **city-team** and place your website in there
  - [ ] WARNING: Do NOT put a **readme.md** file or any other file that's not actually used by the website, on the web server, and make sure the website is installed directly in your city-team folder (not another folder within)!

## Submit the Assignment

*NOTICE:* **EVERYONE** must make a submission in Blackboard

- In the "Assignments Turn-in" area in Blackboard, you'll see a folder titled: **Assignment 3: Information Architecture**
- Within the Assignment 3 folder you will find THREE assignments.  You **pick the one for your role**.  Ignore the others.

As you're making the submission in Blackboard, enter the following in the Write Submission area (*not* the Comments area)

- Click the `Write Submission` button
- In the Text Submission box:
  - Paste a **link to your website**
  - Write your **city-team name**
  - Write a list of **everyone's name** in your team (including your own), and...
  - Next to everyone's name **indicate everyone's role on the team** (IA, designer, or coder)
  - Paste A **link to your team's repository** (which should be set to public)