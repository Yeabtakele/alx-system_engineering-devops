# Web Infrastructure Design

## Description
General
* draw a diagram covering the web stack you built with the sysadmin/devops track projects
* explain what each component is doing
* explain system redundancy
Know all the mentioned acronyms: LAMP, SPOF, QPS
This project is a collection of web infrastructure designs that could be implemented in any web development project.
A lot of websites are powered by simple web infrastructure, a lot of time it is composed of a single server with a LAMP stack.

On a whiteboard, design a one server web infrastructure that hosts the website that is reachable via www.foobar.com. Start your explanation by having a user wanting to access your website.

# Requirements:

You must use:
* 1 server
* 1 web server (Nginx)
* 1 application server
* 1 application files (your code base)
* 1 database (MySQL)
* 1 domain name foobar.com configured with a www record that points to your server IP 8.8.8.8
You must be able to explain some specifics about this infrastructure:
What is a server
What is the role of the domain name
What type of DNS record www is in www.foobar.com
What is the role of the web server
What is the role of the application server
What is the role of the database
What is the server using to communicate with the computer of the user requesting the website
## Designs Presented

+ Simple web stack - [details](0-simple_web_stack.md)
+ Distributed web infrastructure - [details](1-distributed_web_infrastructure.md)
+ Secured and monitored web infrastrucure - [details](2-secured_and_monitored_web_infrastructure.md)
+ Scaled up web infrastructure - [details](3-scale_up.md)
