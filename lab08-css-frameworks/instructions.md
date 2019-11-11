# Lab 8: CSS Frameworks

*Due: Wednesday, November 13, 2019*

In this exercise you will take your Assignment 5 files, rip out the CSS, and then install and use a CSS Framework.  Then you will customize the framework to replicate your original design, as well as possible.

## Step 1: Copy Files

- Copy your Assignment 5 files to a new folder.  (You can name it whatever you want, like **lab08**.)
- UNinstall your current CSS file(s) from your website
  - You can leave your CSS files in the file system.  
  - In all your HTML files, comment-out the **\<link>** tags (don't delete them; you'll need them later)

## Step 2: Install a CSS Framework

- Pick a CSS Framework and learn how to install and use it for formatting and layout
  - Note: this could take a lot of time; just try to cut through it quickly and learn as you go
  - Suggestion: look for tutorials; create a "plain vanilla" test webpage first
- Install the CSS Framework on your Lab 8 files
  - Be sure to install the **\<link>** tags ABOVE the commented-out LINK tags

## Step 3: Use the CSS Framework, as-is

- Apply the framework's CSS classes (and other things, if any, as specified by it's instructions) to your Lab 8 web pages
  - Suggestion: have your Assignment 5 nearby (open in a web browser, or screen shots ...something you can look at) so you can refer to how your website used to look
  - Suggestion: start applying the framework's CSS classes, starting with the layout first (typically the harder part) to the get web page elements to sit where they're supposed to sit in the viewport; then move on to the other formatting and embellishments to try and replicate how your website used to look

## Step 4: Customize the Framework

You can only do so much with the CSS Framework.  At some point you'll have to revert to your own CSS, but having a CSS Framework attached to your website can be problematic.

- Rename your original CSS file(s) to something/anything else; example **styles.css** can become **styles-bak.css** ("bak" short for "back-up")
- Create new/empty CSS files based on your original CSS file names.  E.g. if you had a file named **styles.css** then create a new file named **styles.css** et cetera
- Create a new CSS file named: **override.css** in your CSS folder
- In your HTML, UN-comment-out your **\<link>** tags to your original CSS file(s)
- BELOW all the other CSS **\<link>** tags, create a new link to the new **override.css** file

*Now the real work starts...*

- Open your old CSS files and the new/empty CSS files.  Bit by bit, start copying over CSS styles that do not conflict with the CSS Framework styles.  
  - You'll have to do one at a time; copy & paste then refresh and look; keep going but be sure to NOT use any of your original styles that conflict with the framework's styles

After you've brought over as many styles as you can from your original design, then (and only then!) start writing in your **override.css** file

- Using your browser's **inspector tools** figure out what CSS classes you need to override to incorporate your *conflicted styles*
- Write those CSS properties in your **override.css** file as needed to complete your design

## Turn It In

When your Lab 8 files seem to be working/looking correct, install the lab on our class web server.

- [ ] Open your FTP software and login using the following web server credentials, below.<br>*Note: everyone will use the same FTP account. Be careful not to disturb anyone elses' files.*

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: lab08@csc174.org
FTP Password: [ask the prof]
```

- [ ] When you FTP-in to the account, create a folder using your first initial and last name (e.g. **rkostin** place your application files in there
  - NOTE: as always, DO NOT put your files in a *sub*-subfolder on the web server.  The files need to be in the folder with your name.  You should be able to go to a web address like this: `csc174.org/lab08/flastname/` (where `flastname` is your first initial and last name) and see your lab files right there
- [ ] And of course, go to our CSC 174 section in Blackboard and submit a link to your lab files in the lab assignment named: 

