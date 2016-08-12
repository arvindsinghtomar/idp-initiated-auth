# IDP Initiated Authentication

### Flow Diagram:
![image](https://github.com/arvindsinghtomar/idp-initiated-auth/blob/master/GluuIDPInitiatedAuth.png)

#### Sequence:
  - User logs in to Gluu IDP.
  - User is show the list of websites that are setup with Gluu SP.
  - User can click login button on that website and redirect to Gluu SP with relay_state URL.
  - Validation of SAML Assertion.
  - Dynamic user enrollment if user dosen't exists in SP.
  - Create Gluu server session.
  - Gluu SP redirects user to website 2.
 
First the user is sent to Gluu server IDP where user can login to the system. 
After user is successfully authenticated user is taken to home of Gluu home page. 
On homepage user will be shown the websites which have been set up to work with Gluu SP. 
A user can click on these websites to request that website and will be redirected to Gluu SP where dynamic enrolment of the user will be done if user doesn't exists in the system. 
Then user will be redirected to the website which was requested.

