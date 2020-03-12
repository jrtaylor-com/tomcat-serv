# tomcat-serv

Example setup for a dockerized Tomcat server serving an application.

## Setup

Install Docker https://docs.docker.com/install/

From the repository root directory run ```docker-compose up```

In your browser open http://localhost:8080/sample/

You should now see the Tomcat Hello World sample application.

### Notes 

The ./webapps directory is mounted into /usr/local/tomcat/webapps within the Tomcat container. Replace the contents of that directory with your own application and run the server to interact with your own application.

Additionally a second directory is setup to be served with the hostname ```localhostbackend``` which should be added to your hosts file ```127.0.0.1 localhostbackend``` and then you can access in your browser at http://localhostbackend:8080/sample2/
