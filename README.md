# Developing a Simple Webserver
# Name: vishal 
# Reference Number: 23013753

# AIM:

Develop a webserver to display about top five web application development frameworks.

# DESIGN STEPS:

## Step 1:

HTML content creation is done

## Step 2:

Design of webserver workflow

## Step 3:

Implementation using Python code

## Step 4:

Serving the HTML pages.

## Step 5:

Testing the webserver
# PROGRAM:
```
from http.server import HTTPServer, BaseHTTPRequestHandler

content ="""

 <html>

   <head>

   </head>

   <body>

        <h1>Welcome</h1>

   </body>

 </html>
class HelloHandler(BaseHTTPRequestHandler):

def do_ GET(self):
    self.send_response(200)
    self.send_header('Content-type', 'text/html;charset=utf-8')
    self.end_headers()
    self.wfile.write(content.encode())
server address = ('', 80)

httpd = HTTPServer (server_address, HelloHandler)

httpd.serve_forever()
```
# OUTPUT:
  ![Alt text](image.png)
# RESULT:

The program is executed succesfully
