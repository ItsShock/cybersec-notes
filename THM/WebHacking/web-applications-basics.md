
# web applications basics

**Platform:** TryHackMe  
**Date:** 2026-04-12
**Diff:** Easy

## Tools



## What am learned

A Uniform Resource Locator (URL) is a web address that lets you access all kinds of online content—whether it’s a webpage, a video, a photo, or other media. It guides your browser to the right place on the Internet.

http request/respone, 
HTTP Methods:

GET
Used to fetch data from the server without making any changes. Reminder! Make sure you’re only exposing data the user is allowed to see. Avoid putting sensitive info like tokens or passwords in GET requests since they can show up as plaintext.

POST
Sends data to the server, usually to create or update something. Reminder! Always validate and clean the input to avoid attacks like SQL injection or XSS.

PUT
Replaces or updates something on the server. Reminder! Make sure the user is authorised to make changes before accepting the request.

DELETE
Removes something from the server. Reminder! Just like with PUT, make sure only authorised users can delete resources.

Besides these common methods, there are a few others used in specific cases:

PATCH
Updates part of a resource. It’s useful for making small changes without replacing the whole thing, but always validate the data to avoid inconsistencies.

HEAD
Works like GET but only retrieves headers, not the full content. It’s handy for checking metadata without downloading the full response.

OPTIONS
Tells you what methods are available for a specific resource, helping clients understand what they can do with the server.

TRACE
Similar to OPTIONS, it shows which methods are allowed, often for debugging. Many servers disable it for security reasons.

CONNECT
Used to create a secure connection, like for HTTPS. It’s not as common but is critical for encrypted communication.

request body:
URL Encoded, Form Data, JSON, or XML.

Status Codes:
Informational Responses (100-199)
These codes mean the server has received part of the request and is waiting for the rest. It’s a "keep going" signal.

Successful Responses (200-299)
These codes mean everything worked as expected. The server processed the request and sent back the requested data.

Redirection Messages (300-399)
These codes tell you that the resource you requested has moved to a different location, usually providing the new URL.

Client Error Responses (400-499)
These codes indicate a problem with the request. Maybe the URL is wrong, or you’re missing some required info, like authentication.

Server Error Responses (500-599)
These codes mean the server encountered an error while trying to fulfil the request. These are usually server-side issues and not the client’s fault.



