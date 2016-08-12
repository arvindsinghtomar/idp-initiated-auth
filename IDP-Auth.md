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

### IDP Auth

#### Followed This Link For Shiboleth Config

https://gluu.org/docs/integrate/ubuntu-shib-apache/

##### Response
![image](https://github.com/arvindsinghtomar/idp-initiated-auth/blob/master/ErrorInMataData.png)

#### Followed This Link For Configuring outbound-SAML

https://www.gluu.org/docs/integrate/outbound-saml/

![image](https://github.com/arvindsinghtomar/idp-initiated-auth/blob/master/AddedTrustRelationships.png)

#### For Testing IDP Followed Bellow Link

https://ox.gluu.org/doku.php?id=asimba:saml_script_end_to_end

![image](https://github.com/arvindsinghtomar/idp-initiated-auth/blob/master/IDP%20configuration%20inn%20SP.png)
![image](https://github.com/arvindsinghtomar/idp-initiated-auth/blob/master/Added%20SP%20requester%20in%20IDP.png)

