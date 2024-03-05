Overview       
------------  
                                                                                                              
Start using Galasa to enable deep integration testing across platforms and technologies, and run 
repeatable, reliable, agile testing at scale across your enterprise.  

This zip enables a network-free installation of Galasa, removing the requirement to connect to the 
internet when building or running tests.

This zip file contains:                                                                                                                                                                                                                        
    - A maven directory containing dependencies that are required for building Galasa tests.
    - A javadoc directory containing javadoc API documentation for the Galasa Managers.
    - A galasactl directory containing the binaries of the Galasa CLI.
    - An isolated.tar file - an optional Docker image that hosts the Maven directories. Use this file to host Galasa                        
    on an internal server that can be accessed by other users.
    - A docs.jar file that enables you to run the Galasa website locally on your machine.
                                                                                                 
                                                                                                                                                    
You can find out more about Galasa on the Galasa website https://galasa.dev, or you can host the website locally by 
running the `docs.jar` file that is contained in this zip file on your machine or on an internal server.                                                                

Running the website on your local machine
-------------------------------------------

From a command line, run the following command in the directory in which you extracted the download 
containing the `docs.jar` file: 

`java -jar docs.jar`

The URL to view the locally hosted documentation is returned: http://localhost:9080/


Running the Galasa website on an internal server
----------------------------------------------------
 
To host the website on an internal server so that it can be accessed by other users, set the host 
system properties or environment variables to bind to an externally available network interface, 
rather than localhost. For example: 

`java -Dserver.http.port=12345 -jar docs.jar` or `SERVER_HTTP_HOST=example.com java -jar docs.jar`

 
Getting started 
--------------------                                                                                                                 
                                                                                                                                                   
For information about installing and using the Galasa CLI and getting started with using Galasa, go 
to the "Docs > Getting started using the Galasa CLI" documentation on the Galasa website. 

The locally run website currently links to the external Javadoc site. You can access the Javadoc 
locally by using the Javadoc documentation that is contained in the Javadoc directory provided in this zip. 


Notes
--------------------  

You are responsible for any sensitive information that you put into any configuration files. 