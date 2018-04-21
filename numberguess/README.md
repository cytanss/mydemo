Summary
=======
Demo to show deploying into local EAP vs OpenShift EAP
EAP 7.0

numberguess: Example Using CDI and JSF
=======================================
Summary: The `numberguess` quickstart demonstrates the use of *CDI*  (Contexts and Dependency Injection) and *JSF* (JavaServer Faces) in JBoss EAP.  
Target Product: JBoss EAP  
Original Source: <https://github.com/jboss-developer/jboss-eap-quickstarts/>  

What is it?
-----------

The `numberguess` quickstart demonstrates the use of *CDI*  (Contexts and Dependency Injection) and *JSF* (JavaServer Faces) in Red Hat JBoss Enterprise Application Platform.


Build and Deploy the Quickstart
-------------------------

1. Make sure you have started the JBoss EAP server as described above.
2. Open a command prompt and navigate to the root directory of this quickstart.
3. Type this command to build and deploy the archive:

        mvn clean install wildfly:deploy

4. This will deploy `target/jboss-numberguess.war` to the running instance of the server.


Access the application 
---------------------

The application will be running at the following URL: <http://localhost:8080/jboss-numberguess>. 


Undeploy the Archive
--------------------

1. Make sure you have started the JBoss EAP server as described above.
2. Open a command prompt and navigate to the root directory of this quickstart.
3. When you are finished testing, type this command to undeploy the archive:

        mvn wildfly:undeploy


Debug the Application
------------------------------------

If you want to debug the source code of any library in the project, run the following command to pull the source into your local repository. The IDE should then detect it.

      mvn dependency:sources
