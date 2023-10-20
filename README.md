# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.
![image](https://github.com/knight7080/Ex-04_RESTful_Web_Services/assets/88542035/e11ef614-669a-49a1-a723-5a10f8577076)




Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
 
 ![image](https://github.com/knight7080/Ex-04_RESTful_Web_Services/assets/88542035/bfc93536-d646-47f8-b339-8c9d980aff17)



Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.

![image](https://github.com/knight7080/Ex-04_RESTful_Web_Services/assets/88542035/21525b96-b63f-4523-a4e2-a37b97ddcfea)

Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.
 

 ![image](https://github.com/knight7080/Ex-04_RESTful_Web_Services/assets/88542035/dc033c1b-f4e9-43e0-ad6e-2001f1d671a2)



Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.


![image](https://github.com/knight7080/Ex-04_RESTful_Web_Services/assets/88542035/eef7ab2b-6954-45f5-84d1-3c875a133cdc)


Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. 
Step 4: Carefully select your RESTful resource (web service) and click OK.
![image](https://github.com/knight7080/Ex-04_RESTful_Web_Services/assets/88542035/210ee94e-f404-4815-a16b-a434dbb2e7d5)
 
 


Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.
![image](https://github.com/knight7080/Ex-04_RESTful_Web_Services/assets/88542035/4cb7a436-668e-4988-bfd0-bee28a36087b)


Step 6: An editing tab will open. Alter getHtml() method with the following.
 
 ![image](https://github.com/knight7080/Ex-04_RESTful_Web_Services/assets/88542035/c5e5bbe3-7e9a-44aa-bac6-3c170f94cddc)



Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.
![image](https://github.com/knight7080/Ex-04_RESTful_Web_Services/assets/88542035/18ba6caa-caf2-45e1-8066-735ca6afe6d1)


Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 ![image](https://github.com/knight7080/Ex-04_RESTful_Web_Services/assets/88542035/4a01c0d0-417a-4c80-94d1-fe962cf0907e)

 


Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.
![image](https://github.com/knight7080/Ex-04_RESTful_Web_Services/assets/88542035/0a2077ee-aa7d-4bed-87bd-c2c118e4784b)


Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.
 ![image](https://github.com/knight7080/Ex-04_RESTful_Web_Services/assets/88542035/730c806b-028a-4d52-9b84-a19a64e0b043)

 


Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
