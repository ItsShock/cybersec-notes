# Networking core protocols

**Platform:** TryHackMe  
**Date:** 2026-03-21
**Diff:** Easy

## Description


## What am learned
A, AAAA, and MX , WHOIS 

http/https
-GET retrieves data from a server, such as an HTML file or an image.
-POST allows us to submit new data to the server, such as submitting a form or uploading a file.
-PUT is used to create a new resource on the server and to update and overwrite existing information.
-DELETE, as the name suggests, is used to delete a specified file or resource on the server.

FTP
-USER is used to input the username
-PASS is used to enter the password
-RETR (retrieve) is used to download a file from the FTP server to the client.
-STOR (store) is used to upload a file from the client to the FTP server.

SMTP
-HELO or EHLO initiates an SMTP session
-MAIL FROM specifies the sender’s email address
-RCPT TO specifies the recipient’s email address
-DATA indicates that the client will begin sending the content of the email message
-. is sent on a line by itself to indicate the end of the email message

POP3:
Some common POP3 commands are:
-USER <username> identifies the user
-PASS <password> provides the user’s password
-STAT requests the number of messages and total size
-LIST lists all messages and their sizes
-RETR <message_number> retrieves the specified message
-DELE <message_number> marks a message for deletion
-QUIT ends the POP3 session applying changes, such as deletions

IMAP:
-LOGIN <username> <password> authenticates the user
-SELECT <mailbox> selects the mailbox folder to work with
-FETCH <mail_number> <data_item_name> Example fetch 3 body[] to fetch message number 3, header and body.
-MOVE <sequence_set> <mailbox> moves the specified messages to another mailbox
-COPY <sequence_set> <data_item_name> copies the specified messages to another mailbox
-LOGOUT logs out

TELNET  protocol is a network protocol for remote terminal connection


