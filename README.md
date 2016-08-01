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
  - SP redirects user to website 2.
