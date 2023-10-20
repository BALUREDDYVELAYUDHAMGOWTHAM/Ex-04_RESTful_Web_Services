# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.


![ex03_01](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-04_RESTful_Web_Services/assets/119559905/d373199d-6217-44b5-a1b8-b46a9e9c4896)


Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
 
 
![ex03_02](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-04_RESTful_Web_Services/assets/119559905/31f7efbd-ba9f-4ee9-966e-ffb0d31e54a3)


Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.

![ex03_03](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-04_RESTful_Web_Services/assets/119559905/eb5725c3-989a-4098-9356-cccafb12c7f8)

Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.

Step 6: Alter getHtml() method as shown below.

Step 7: Save your project, clean and build it. Deploy your project.
 

 
![ex03_04](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-04_RESTful_Web_Services/assets/119559905/881e6734-33db-4e61-8232-c3c1cd3ad0f5)


Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



### Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.

![ex03_05](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-04_RESTful_Web_Services/assets/119559905/2221286d-88c5-4730-9e5c-9441905ed41a)


Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. 

Step 4: Carefully select your RESTful resource (web service) and click OK.
 


![ex03_06](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-04_RESTful_Web_Services/assets/119559905/b71689de-9318-4b2a-ba33-657b60ebea08)


Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.
 ![ex03_07](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-04_RESTful_Web_Services/assets/119559905/5a638789-76cd-4e6e-8e0d-93f2e680c939)


Step 6: An editing tab will open. Alter getHtml() method with the following.
 
 ![ex03_08](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-04_RESTful_Web_Services/assets/119559905/4076da6b-ee79-4ffe-82f3-63daa536b853)



Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.
![ex03_09](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-04_RESTful_Web_Services/assets/119559905/f565676e-bf24-4f2c-9035-83d957e0f11f)


Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 
 ![ex03_10](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-04_RESTful_Web_Services/assets/119559905/1ea59045-7880-415d-a7d6-180a8b0a8435)




Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.

Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.

![ex03_11](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-04_RESTful_Web_Services/assets/119559905/4a668af1-7a9d-485d-ab47-d400a7742a1b)

Step 11: Save the project and build it.

Step 12: Run the JSP file and you should see the output in a new browser window.
 
 ![ex03_12](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-04_RESTful_Web_Services/assets/119559905/5783c8d6-6573-4f4d-ac38-b43c35b94702)



### Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2

Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";

Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
