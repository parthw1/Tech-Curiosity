# Notes

## WSGI - WSGI is the Web Server Gateway Interface

* It is a specification that describes how a web server communicates with web applications, and how web applications can be chained together to process one request.
* It is a simple calling convention for web servers to forward requests to web applications or frameworks.
* Java's "servlet" API makes it possible for applications written with any Java web application framework to run in any web server that supports the servlet API.
* WSGI was thus created as an implementation-agnostic interface between web servers and web applications or frameworks to promote common ground for portable web application development.
* Imp link -- https://www.cabotsolutions.com/2017/11/a-detailed-study-of-wsgi-web-server-gateway-interface-of-python

## WSGI Middleware
* A WSGI middleware component is a Python callable that is itself a WSGI application, but may handle requests by delegating to other WSGI applications. These applications can themselves be WSGI middleware components.
* A middleware component can perform such functions as:
  - Routing a request to different application objects based on the target URL, after changing the environment variables accordingly.
  - Allowing multiple applications or frameworks to run side-by-side in the same process
  - Load balancing and remote processing, by forwarding requests and responses over a network
  - Performing content post-processing.
  
