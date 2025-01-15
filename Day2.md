# Web Exploitation


# HTTP Response Codes

- 10X = Informational

- 2XX = Success

- 30X = Redirection

- 4XX = Client Error

- 5XX = Server Error
# Enumeration

- Robots.txt: list off different directorys contained in web server
# Cross-Site Scripting (XSS) Overview
- Allows us to arbitaurily place code on a webpage
-
- <script>alert('XSS');</script>

# Reflected XSS

- Deliver something to server and someone clicks it similiar to phishing through a email

- You put the vulnerability on the server and someone else interacts with it
# Stored XSS

- Already on server and know how to exploit

- The server already has the vulnerability and you interact with it

# Malicious File Upload

- Site alows unsanitized file uploads

- Does not check extension, Allows for code execution

