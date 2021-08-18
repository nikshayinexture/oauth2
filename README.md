# oauth2
Login With Your Google Account with Open Authorization 2.

1.In Security Config we've authorized API call request with oatuh2Login.

2.We've created two APIs in the application file itself, to access these APIs we need to login using google id.

3.Before testing our application we first need to create the google cloud credentials to enable google login and mention the credentials in the application.yml file in main/resources.

4.Visit console.cloud.google.com to create new credentials, click on API and Services.

5.Enter credentials tab from the sidebar and create OAuth2 Client ID by clicking on Create Credentials button.

6.As we are creating a web application select web app and give a app name of your choice.

7.Add URI and redirect URI 
Ex: 
URI : http://localhost:8089

Redirect URI : http://localhost:8089/login/oauth2/code/google

After saving you'll get a ClientID and Client Secret.

8.Update the application file  with these Credentials.

9.Run your application file as a Spring Boot Project.

10.Visit http://localhost:8089/ in your browser

11.Enter your google id to login

Output : You're Succesfully Logged In With Google

12.Enter http://localhost:8089/user in browser to access the API which will return the user information from google which can be used to create a new account on our web app.

