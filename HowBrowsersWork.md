# How Browsers Work
# Introduction
We all know what browsers are and what they do. However, many of us do not know how they function in the background. Browsers are, by far, the most used software. As a Web developers, you do need to know the mechanics of how browsers work behind the scenes. We will see what happens when you type in a search such google.com in the address bar until you see the google page on the browser window. That knowledege would help you to decipher the justifications behind development best practices.
# Major Browsers
There are a lot of browsers to choose from (both desktop and mobile). There are five major browsers used for desktops today: Firefox, Chrome, Safari, Inernet Explorer (IE), and Opera. Major browsers in use for mobile: Android Browser, iPhone, Opera Mini and Opera Mobile, UC Browser, the Nokia S40/S60 browsers and Chrome. As of June, 2013, Chrome, Firefox and Safari make up 71% of global desktop browser usage, according to StatCounter Statistics. Android, iPhone, and Chrome made up 54% of usage on mobile.
# Browser's Main Functionality
The main functionality of a browser is to present the web resource you choose by requesting it from the server and displaying it on your browser window. The resource is usually an html document but could also be PDF, image, or some other type of content. The location of the resource is spcified by the user using a URI (uniform resource identifier).
The way the browser interprets and displays HTML files is specified in the HTML and CSS specifications that are maintained by w3C (World Wide Web Consortium) Organization. Although this has not always been the case, most of the browsrs more or less conform to the specification.
Browser user interfaces have a lot in common and consist of the following:
    - Address bar for inserting a URI
    - Back and forward buttons
    - Bookmarking options
    - Refresh and stop buttons for refreshing or stopping the loading of current documents
    - Home button that takes you back to your home page
Browser interfaces are not specified in any formal specification. Although HTML5 specifications does not define any UI elements a browser must have, it does list some common elements. Among these elements are Address Bar, Status Bar, and Tool Bar.
# How browsers Functions
    - As soon as you type in a web address into your browser's address bar, some communication starts to occurs
    - The browser sends an HTTP request through the internet to where the server that runs the website is located
    - the web server then sends back an HTTP response which is read by the browser to display the site
    - the response contains the website in HTML form, which the browser translates and displays the complete site as we view them
HTTP Requests
Contain 3 Parts:
    1. Request line: command, web page requested, HTTP version number
    2. Request header: includes browser in use, date, and some other info
    3. Request body: contains information that was sent to the server (optional)
Below is an Example Request:
GET             Salisbury/home.html             HTTP/1.1
Host:www.su.edu                                 Request line
Date: Tues 08 Sept 2006 13:45:34 EST
User-Agent: Mobile/7.0
Referrer: http:salisbury.edu/~welcome
HTTP Response
Contains 3 parts:
    1. Response status: http version#, status code, and response phrase (description of status code)
    2. Response header: optional info including server being used, date, URI of web page
    3. Response body: the website (in html)
    HTTP/1.1                200                 ok                          Response status
    Date: Tues 08 Sept 2006 13:45:34 EST
    Server: Apache
    Location: http:salisbury.edu/rtduany/~welcome                           Response header
    content-type: text/html
    <html>
    <head>
    <title>Salisbury></title>
    </head>
    <body>
    <p>welcome to salisbury</p>
    -----
    </body>
    </html>                                                                Response body in HTML
    Amazingly, this whole process takes less than 1 second depending on your internet connection.