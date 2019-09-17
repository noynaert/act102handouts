# Shortcuts and Helpers

## Shortcuts you should practice and know

These shortcuts should work in Windows 10 and most Linux distributions.  Some will work for Macs.

* Ctrl-s : Saves the current file
* Ctrl-a : Selects everything.  This works with most applications that use text.  It is very handy when you want to move an entire web page or style sheet.
* Ctrl-c : Copies selected text
* Ctrl-v : Pastes text
* Ctrl-x : Cuts text and puts it on the clipboard
* Ctrl-z : Undo (may be repeated)
* Alt-tab: Switch between applications

## Tiling the screen

It is often handy to have your text editor on the left half of your screen and a browser on the right.  These shortcuts should do it for you.  The "Super" key is the Windows key between the Ctrl and Alt keys on most keyboards.  (If you tile VS Code be sure to close the File flyout to give yourself more room.)

* Super-LeftArrow: Tiles the current app on the left half of screen
* Super-RightArrow: Tiles the current app on the right half of the screen

## Triple Click

In most text applications triple-clicking the mouse will select the current paragraph

## Uploading files to the P: drive from home

There are three methods with increasing levels of sophistication required.

### Easy but cumbersome method: Webservices

Go to https://webservices.missouriwestern.edu.  Click on "Serve-U."  This should take you to your p:\ drive root.  Click on "public_html" and then on your act102 folder.  You may use the links to upload and download.

### Somewhat easier but more technical method: SFTP gui client

Download a gui ssh or sftp client such as [Bitvise](https://www.bitvise.com/download-area).  The host name will be webservices.missouriwestern.edu.  If it gives you a choice of protocol, select "SFTP."  If the client asks for a port use port 22.

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
Note that this file ***must*** go in the root of the ACT102 folder on your local system.