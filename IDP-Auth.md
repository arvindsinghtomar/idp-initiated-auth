### IDP Auth

There are two setups of Gluu server
1. https://gluu.local.org
2. https://gluu.idp.org

Here https://gluu.local.org works as SP and https://gluu.idp.org is configured as IDP.

#### Followed This Link For Shiboleth Configuration
https://gluu.org/docs/integrate/ubuntu-shib-apache/

Followed all the steps in the link for configuration.
After completeing all the steps, testing the printHeaders.py script didn't gave any error and instead it prints the script itself and now it is giving this error unable to locate metadata for IDP.

##### Error
![image](https://github.com/arvindsinghtomar/idp-initiated-auth/blob/master/img/ErrorInMataData.png)

#### Followed This Link For Configuring outbound-SAML
Followed all the steps in this link for configing outbound-saml

https://www.gluu.org/docs/integrate/outbound-saml/

Addes trust relationship with IDP (gluu.idp.org)
![image](https://github.com/arvindsinghtomar/idp-initiated-auth/blob/master/img/AddedTrustRelationships.png)

#### Followed This Link For Configuring inbound-SAML
Followed all the steps in this link for configing inbound-saml

https://www.gluu.org/docs/integrate/inbound-saml/

Added IDP
![image](https://github.com/arvindsinghtomar/idp-initiated-auth/blob/master/img/IDP%20configuration%20inn%20SP.png)

Added SP requester
![image](https://github.com/arvindsinghtomar/idp-initiated-auth/blob/master/img/Added%20SP%20requester%20in%20IDP.png)

Added SP selector
![image](https://github.com/arvindsinghtomar/idp-initiated-auth/blob/master/img/SAMLSelector.png)

#### For Testing And Configuring IDP Followed Bellow Link
https://ox.gluu.org/doku.php?id=asimba:saml_script_end_to_end

After configuration according to this link, facing the same problem agin unable to locate metadata for IDP.

##### Error
![image](https://github.com/arvindsinghtomar/idp-initiated-auth/blob/master/img/ErrorInMataData.png)




