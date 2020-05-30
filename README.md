# Power BI Embed Token Asp.net Rest API SourceCode
Asp.net Rest API Power BI Embed token Generates an embed token to view the specified dashboard from the specified workspace.

## Setting up the Power BI and Azure Environment
Create PowerBI App in Azure using https://dev.powerbi.com/apps and assign appropriate permission for reports. 
![Register Power BI Azure APP](https://github.com/stw-services/PowerBIembedTokenSourceCode/blob/master/PowerBIEmbedded_AppOwnsData/images/AppRegistration.PNG)

## Assign Api Permission in Azure 
Login to http://portal.azure.com/, got Active Directory and App Registration part and select created App. In left navigation select API Permissoin. And Grand Admin consents. Also if you are getting error - AADSTS65001: The user or administrator has not consented to use the application....

![Grand Admin Consents](https://github.com/stw-services/PowerBIembedTokenSourceCode/blob/master/PowerBIEmbedded_AppOwnsData/images/Grant%20Admin%20Consents.PNG)

## AADSTS7000218: The request body must contain the following parameter: 'client_assertion' or 'client_secret' 
IF you are getting this error verify redirect url and and Default client type. Redirect url must be same from which you are callling api. 
![Redirect URL](https://github.com/stw-services/PowerBIembedTokenSourceCode/blob/master/PowerBIEmbedded_AppOwnsData/images/RedirectURL.PNG)

### Default client type
![Default client type](https://github.com/stw-services/PowerBIembedTokenSourceCode/blob/master/PowerBIEmbedded_AppOwnsData/images/Implicit%20Grant.PNG)

For PowerBI consultation connect us on info@softechworld.com
