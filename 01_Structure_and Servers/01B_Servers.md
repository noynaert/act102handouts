# 01B Servers

The internet hosts two types of computers -- Clients and Servers.

## Clients

Browsers such as Chrome, Firefox, Edge, Internet Explorer, and Safari are clients.  Clients usually only run when a human user wants to pull something off the Internet (or forgets and leaves their computer on).

## Servers

Servers typically run 24 hours a day, 365 days a year. They sit and wait for a client to contact them and request information.

Servers often do not have keyboards or monitors permanently attached.  They often reside in data centers.

| A server being installed in a rack|Server racks in a data center|
|:---:|:---:|
|![Server in a rack](images/Rackmount-Server.jpg)|![A Data Center ](images/google-people-14-e1402017295557.jpg)|
| |Human for scale|

## Servers on our campus

We actually have a lot of servers on our campus.

### Mini-exercise

* Visit http://turing.cs.missouriwestern.edu/
* Hold down the Ctrl key and press "u".  (On Windows or Linux, not sure about a Mac)
* You should now see the "source code" for the page.  
  * You should understand what most of the tags are.
  * What is the title of the page?  Does the title show up anywhere?  If so, where?
  * Does the page have any header tags?
  * What would you guess the &lt;style&gt; tag does?
  * Is the style in the head or body of the document?
  * Inside the style tag there is some CSS.  
    * We will cover CSS in a few weeks.  
    * CSS is concerned with the appearance of the document.  HTML is concerned with the structure.

## The P: drive

The P: drive is a drive on campus computers.  The P: drive is only available on campus.  There are ways to get to it from off campus, but they are harder than on campus.  This is why I suggest doing the first couple of assignments from on campus.  I will show you how to get to it in a couple of weeks when you will not be so overwhelmed by other things in the class.  Also, I hope you will have developed a higher threashold for frustration by that point. :smirk:

Your P: drive should have a directory called P:\public_html.

### Mini exercise

* Open a browser.  Go to the following url, except put in your own email address instead of XXXXX  http://webservices.missouriwestern.edu/users/XXXXX  You should see the contents of your folder.
* Using the Windows file explorer, copy your aboutMe.html file into the p:\public_html folder.
* Refresh your browser.  You should see the aboutMe.html file.  Click on it and you should see your web page.
* Using Windows file explorer, right click in the P:\public_html folder and create a file called "homework" (no quotes, and make it all lower case.)
* Go back to the browser and refresh.  You should now see the homework folder along with your aboutMe.html folder.
* Open a new tab in your browser.  In the new tab put in the url of the person sitting next to you.  You can now see their files as well.  In fact, anyone on the Internet can rummage through your files.  This is not necessarily a good thing.
* In Windows file explorer, right click on aboutMe.htm.  Rename the file "index.html" without the quote marks.  Refresh your browser.
* ***index.html is a "magic file name."  When the server software sees a file named index.html or index.php it will display that file instead of the entire directory contents.  index.html becomes the landing page for your directory***
* Review your index.html to make sure there is no confidential information.  Use VS Code to edit the file if there is any confidential information or anything you do not want to show up on the Internet.  Save the file and refresh your browser.
* If you really want privacy copy the source code from the turing.cs.missouriwestern.edu landing page and use that for your index.html page.  It is your choice.

## Things to know

* What is client software? Give some examples.
* What is a server?  How is a computer running a server different than a computer running a client?
* What is the significance of the file name index.html?
* What is a landing page?
  