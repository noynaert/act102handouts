# Uploading

## Uploading files to the P: drive from home

There are three methods with increasing levels of sophistication required.

### Easy but cumbersome method: Webservices

Go to https://webservices.missouriwestern.edu.  Click on "Serve-U."  This should take you to your p:\ drive root.  Click on "public_html" and then on your act102 folder.  You may use the links to upload and download.

### Somewhat easier but more technical method: SFTP gui client

Download a gui ssh or sftp client such as FileZilla.  If you are on a Windows or Mac system make sure you only get this from [https://filezilla-project.org/](https://filezilla-project.org/)  There are many versions of FileZilla that are loaded with malware.  If you are using Linux you should only download FileZilla from the repositories that are default for major distributions.

Start FileZilla.  It should show "Local site" which is your computer.  Ont the right there is the Remote site.  But this is empty because you are not connected to anything.

To set up a connection:

1. Click on "File/Site Manager"
2. Click "New site"
3. Fill in the required fields
   * Host is webservices.missouriwstern.edu
   * Port is 22
   * Protocol should be SFTP - SSH File Transfer Protocol
   * Set login Type to "Ask for password"
   * Put in your user name
   * I changed the background color to yellow, just to make it easier to see which was the remote site.  
4. Click OK.
5. Optional: Open site manager again and select "New site." Then click on "Rename""  Change it to "Webservices"

You may now go back to the main screen and click on "Quickconnect."  Select sftp://webservices.missouriwestern.edu

Put in your password.  The first time you connect it will give you a warning about the host key being unknown.  Check the "Always trust" box.

The host name will be webservices.missouriwestern.edu.  If it gives you a choice of protocol, select "SFTP."  If the client asks for a port use port 22.

In most clients the "remote" will be webservices while your "local" system will be your laptop or PC.

If you use this method you should make an act102 folder on your computer.  Then download your entire p:\public_html\act102 folder.  Then edit the files on your local server.  When you are finished editing sync your local folder to the remote folder.

### Most technical, but easiest after you get it working: SFTP in VS Code

Do not even think about using this method unless you open folders, not files!

Open the "Extensions" flyout on the left side of VS Code.  Search for SFTP.

I have been using SFTP/FTP sync by liximomo.

After you have downloaded it, move to your ***local*** act102 folder.  Then do either F1 or Ctrl-Shift-P.  Search for SFTP: Config

Edit the JSON file.  Mine looks like this: 

```text
{
    "name": "ACT 102 ",
    "host": "webservices.missouriwestern.edu",
    "protocol": "sftp",
    "port": 22,
    "username": "noynaert",
    "remotePath": "/public_html/act",
    "uploadOnSave": true
}
```

After this is set up, do either F1 or Ctrl-Shift-P to open the menu.  Select "

Note that this file ***must*** go in the root of the ACT102 folder on your local system.