## 0x09. Web infrastructu

* I have be able to draw a diagram covering the web stack you built with the sysadmin/devops track project
* I have  able to explain what each component is doing
* able to explain system redundancy
Know all the mentioned acronyms: LAMP, SPOF, QPS
## Files

<summary><a href="./0-simple_web_stack.jpg">0. Simple web stack</a></summary><br>

<summary><a href="./1-distributed_web_infrastructure.jpg">1. Distributed web infrastructure</a></summary><br>

<summary><a href="./2-secured_and_monitored_web_infrastructure.jpg">2. Secured and monitored web infrastructure</a></summary><br>

<summary><a href="./3-scale_up.jpg">3. Scale up</a></summary><br>
### This project contains tasks for learning more about the different ways a web infrastructure could be designed for web development.
# web stack
mandatory
A lot of websites are powered by simple web infrastructure, a lot of time it is composed of a single server with a LAMP stack.
On a whiteboard, design a one server web infrastructure that hosts the website that is reachable via www.foobar.com. Start your explanation by having a user wanting to access your website.
Requirements:
# You must use:
* 1 server
<S-F8>1 web server (Nginx)
* 1 application server
* 1 application files (your code base)
* 1 database (MySQL)
* 1 domain name foobar.com configured with a www record that points to your server IP 8.8.8.8
#You must be able to explain some specifics about this infrastructure:
* What is a server
* What is the role of the domain name
* What type of DNS record www is in www.foobar.com
* What is the role of the web server
* What is the role of the application server
* What is the role of the database
What is the server using to communicate with the computer of the user requesting the website
You must be able to explain what the issues are with this infrastructure:
SPOF
Downtime when maintenance needed (like deploying new code web server needs to be restarted)
Cannot scale if too much incoming traffic
### Distributed web infrastructure
mandatory
On a whiteboard, design a three server web infrastructure that hosts the website www.foobar.com.
Requirements:
#1 database (MySQL)
You must be able to explain some specifics about this infrastructure:
For every additional element, why you are adding it
What distribution algorithm your load balancer is configured with and how it works
Is your load-balancer enabling an Active-Active or Active-Passive setup, explain the difference between both
How a database Primary-Replica (Master-Slave) cluster works
What is the difference between the Primary node and the Replica node in regard to the application
You must be able to explain what the issues are with this infrastructure:
Where are SPOF
Security issues (no firewall, no HTTPS)
No monitoring
###. Secured and monitored web infrastructure
Secured and monitored web infrastructure
mandatory
On a whiteboard, design a three server web infrastructure that hosts the website www.foobar.com, it must be secured, serve encrypted traffic, and be monitored.
Requirements:
You must add:
3 firewalls
1 SSL certificate to serve www.foobar.com over HTTPS
3 monitoring clients (data collector for Sumologic or other monitoring services)
. Scale up
#advanced
Readme

Application server vs web server
Requirements:

You must add:
1 server
1 load-balancer (HAproxy) configured as cluster with the other one
Split components (web server, application server, database) with their own server
You must be able to explain some specifics about this infrastructure:
For every additional element, why you are adding it
