Explore the store as described in the documentation page [Explore the Store | SAP Help Portal](https://help.sap.com/docs/PROCESS_AUTOMATION/527c579a1cba4f12b45326c8e890d102/b38897b821874ebe98fb15fc7d4400e9.html?locale=en-US)

We will be searching for SuccessFactors Offer Letter Automation.

1. As a first step, we will download Offer Letter Automation Bot from the RPA Store. Here I will share generic instructions to download any bot business content from the store. [Get a Store Package | SAP Help Portal](https://help.sap.com/docs/IRPA/c8e1e1d0e82547d4b4c926563984a1e5/8beb0ce5799a4b31b389fe11939ef614.html?locale=en-US) 
2. Ddeploy the package immediately for testing. You can use this documentation page for additional information [Deploy a Store Package Immediately for Testing | SAP Help Portal](https://help.sap.com/docs/IRPA/c8e1e1d0e82547d4b4c926563984a1e5/a39a5b0ae11045559bea087e47d73fec.html?locale=en-US)
3. The environment variables you will find at the time of deployment is what the bot expects as input to successfully execute the business content. You will need to fill relevant data as per your SuccessFactors Tenant configurations

Name | Description | Type | Sample | is it Mandatory?
------------ | ------------ | ------------ | ------------| ------------
apiURL| [API URL of SuccessFactors (see KBA 2215682)](https://userapps.support.sap.com/sap/support/knowledge/en/2215682) |String | [https://apisalesdemo4.successfactors.com:443/odata/v2](https://apisalesdemo4.successfactors.com/odata/v2)| Required
botuser| Bot user username and password |Credential | botuser/password| Required
companyId| CompanyID of the SuccessFactors instance |String | SFPART012345| Required
botStep| Applicant status where candidates will be placed to be picked up by the bot |String | Request Offer Letter| Required
OfferType| Offer type the bot will send. Options are: 1) Online offer (2) Verbal offer (3) Email as text (4) Email as PDF attachment |String | SPA Automation added prescreen questions| Required
sfurl| SuccesFactors application URL |String | [https://salesdemo4.successfactors.com/](https://salesdemo4.successfactors.com/)| Required
outputFolderPath| Folder Path to save bot execution logfile |String | C:\Temp| Optional
logEmail| Email that will receive bot execution logs |String | [sfadminEmail@bestRunSAP.com](mailto:sfadminEmail@bestRunSAP.com)| Optional
inputFilePathSFOfferLetter| Input File Path (Only required when you are triggering SF_Offer_Letter_UI_Only_Start Automation) |String | C:\Temp\Input| Optional

Depending on your chosen trigger, bot will automatically trigger for Scheduled triggers or it will be ready to run for Attended triggers.