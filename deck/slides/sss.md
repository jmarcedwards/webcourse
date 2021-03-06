# Server-side scripting

!SLIDE
# Server-side scripting

!SLIDE
>Server-side scripting is a technique used in website design which involves embedding scripts in an HTML source code which results in a user's (client's) request to the server website being handled by a script running server-side before the server responds to the client's reques. [*Wikipedia*](http://en.wikipedia.org/wiki/Server-side_scripting)

!SLIDE
### Dynamics web page
![Dynamic page](images/Scheme_dynamic_page_en.svg)

!SLIDE left
## Scripting
* Embed simple code in HTML pages.
* The HTML pages use the code to decide what elements to display and what data should be displayed.
* Existing APIs can be invoked to compute information for inclusion in the web page.

!SLIDE left
## Key components of Server-Side Scripting
* Web Server
* Server-side processor - interprets scripts and generates HTML

!SLIDE left
## Apache web server
* Apache http server project
* http://httpd.apache.org
* Apache foundation started to support the web server project, but now extends to a multitude of other projects.

!SLIDE
## Demo: configuring Apache to work with PHP
!NOTE edit /private/etc/apache2/httpd.conf

!SLIDE
### Configure directory DocumentRoot - the directory out of which web server will serve the documents (html, php, etc). By default, all requests are taken from this directory.
#### DocumentRoot "/Library/WebServer/Documents"

!SLIDE
## What if we open PHP file in the browser?
![PHP](images/php_plain.png)

!SLIDE
## Apache *php5_module* should be enabled to handle *.php files
#### In the httpd.conf: LoadModule php5_module libexec/apache2/libphp5.so

!NOTES
1. enable LoadModule php5_module libexec/apache2/libphp5.so          2. sudo apachectl restart
3. http://localhost/index.php                                        
                                                                     
!SLIDE
![Apache](images/apache.png)

!SLIDE
>PHP is a general-purpose server-side scripting language originally designed for Web development to produce dynamic Web pages. It is one of the first developed server-side scripting languages to be embedded into an HTML source document rather than calling an external file to process data. The code is interpreted by a Web server with a PHP processor module which generates the resulting Web page.

!SLIDE 
## PHP Flow
![](images/php_flow.png)

!SLIDE
![](images/webProg/php1.png)

!SLIDE
TODO: more on Scripting in PHP
loop generating a table from PHP array

!SLIDE 
### DEMO [101implementation:PHP](http://101companies.org/index.php/101implementation:php)

!SLIDE left
## Summary
### You learned
* the priciples behind Server-Side Scripting
* about the role of web server in web applications
* Apache web server basic configuration
* how generate dynamic web pages with PHP

!SLIDE left
## Resources
* [http://www.w3schools.com/php/default.asp](http://www.w3schools.com/php/default.asp)
