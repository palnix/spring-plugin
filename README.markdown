# Palnix Live Update (PLU)

## Preface

### Introduction

HTML is by far the most popular language when it comes to developing web pages and as designers
being able to see changes straight away in the browser is core for speedy development and instant
feedback. 

### Context
PLU is a tool that gives you a snappy and responsive development environment
that gives you instant feedback whilst you are creating your websites. Rather than having to
update your code, refresh the browser and wait to the changes to display, PLU monitors your
project directory and updates your browser in realtime so that you see the changes immediately.

There are of course, alternative software available that do exactly the same thing, however
PLU is a far better for the following reasons:

-   Automatically reloads the web browser when a change is detected in HTML/JavaScript code.
-   Without refreshing the browser: Automatically updates modified images and CSS files.
-   Uses WebSockets: Unlike traditional methods of polling, WS allows for extremely low latency 
and is the magic behind the dynamic content updating.
-   No sourcecode modifications required! Code is injected by PLU during runtime, so your files are unaffected.
-   PLU ships with a built-in Web Server to serve your web files. You can use your own web server! Just include the palnix.js in your code.
-   The code is open source, so you can do whatever you want subject to the EPL-2.0 License.

## Setup

### Prerequisites 
-   Java 11 is required to launch Live Update. Install Java from http://java.com/
-   Optional: A web server if you decide not to use the built in version

### Installation
1. Download the palnix.jar from http://palnix.com/live-updates/palnix-live-update.jar
2. Launch Live Update via Terminal or Command Prompt using the command 

   ```java -jar palnix-live-update.jar root="/www/myapp"```
   
   Remember: Replace /www/myapp with the Path to your websites directory.
   
Need help? You can see details by running 

```java -jar palnix-live-update.jar help```

## List of all available runtime arguments

| arg  | Description |
| ------------- | ------------- |
| root  | Required: The directory containing your web files.
| port  | Optional: The port to run the web server on. Default: 8080 
| enableWebServer  | Optional: Should the http server be running? Default: true

## Libraries
The following libraries are used in this project:

-   Vertx 3.9.2
-   Log4j 2.13.3
-   JUnit 4.13


