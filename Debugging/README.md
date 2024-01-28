Deconstructing journey of an HTTP request

Activity

Click on the request for the HTML file. (Find the entry In the Name tab, you should see www.flipkart.com with Type as document).


Details of an HTTP Request


Observe the following details for this HTTP request in the “General” section
Request URL
Request Method
Status Code
Remote Address


These properties calls out some important information regarding the request-response process for a request

Request URL → URL of the resource fetched (what you typed in the Browser’s URL bar)
Request Method → Action to be done. “GET” is for downloading (getting) some resource
(Response) Status Code → How the server responded to the request
“200 OK” means a successful request
As this is a successful “GET” request, server will have sent some data back i.e, website’s HTML content




Remote Address → Address of the application serving the resource requested. Has two sections
IP address → Location of the server hosting the resource (eg: 163.53.78.128)
Port → Location of the application within the server, serving the resource (eg: 443)

HTTPS ==> 443
HTTP ==> 80

Browser uses the URL you typed to figure out the Remote address of the server.



Activity

Try opening couple more websites like you did for https://www.flipkart.com/ (i.e, load page, open Developer Tools, refresh page)
https://www.google.co.in/
https://www.crio.do/testimonials/
Check the IP and Port values of the servers from the “Remote Address” property. Any interesting observations?
Is there any relationship between the port number used and the Request URL?

Activity
Check out the properties in the Response Headers section of the “Headers” tab
See if you can find out what some of these mean eg: Content-Type, Server

Curious Cats
Visit https://www.flipkart.com and http://pizza.com. What are the Port numbers these two servers use? Are they the same? Why is there a lock icon on the address bar of one of these websites but not the other?

