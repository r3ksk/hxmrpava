Explore the store as described in the documentation page [Explore the Store | SAP Help Portal](https://help.sap.com/docs/PROCESS_AUTOMATION/527c579a1cba4f12b45326c8e890d102/b38897b821874ebe98fb15fc7d4400e9.html?locale=en-US))

We will be searching for SuccessFactors Pre-Screen questions Automation.

1. As a first step, we will download Pre-Screen Questions Bot from the RPA Store. Here I will share generic instructions to download any bot business content from the store. [Get a Store Package | SAP Help Portal](https://help.sap.com/docs/IRPA/c8e1e1d0e82547d4b4c926563984a1e5/8beb0ce5799a4b31b389fe11939ef614.html?locale=en-US) 
2. Ddeploy the package immediately for testing. You can use this documentation page for additional information [Deploy a Store Package Immediately for Testing | SAP Help Portal](https://help.sap.com/docs/IRPA/c8e1e1d0e82547d4b4c926563984a1e5/a39a5b0ae11045559bea087e47d73fec.html?locale=en-US)
3. The environment variables you will find at the time of deployment is what the bot expects as input to successfully execute the business content. You will need to fill relevant data as per your SuccessFactors Tenant configurations

Name | Description | Type | Sample | is it Mandatory?
------------ | ------------ | ------------ | ------------| ------------
apiURL| [API URL of SuccessFactors (see KBA 2215682)](https://userapps.support.sap.com/sap/support/knowledge/en/2215682) |String | [https://apisalesdemo4.successfactors.com:443/odata/v2](https://apisalesdemo4.successfactors.com/odata/v2)| Required
sfuser| Bot user username and password |Credential | botuser/password| Required
companyId| CompanyID of the SuccessFactors instance |String | SFPART012345| Required
completedComment| Comment to be added when moving the job requisition tot he next step |String | SPA Automation added prescreen questions| Required
questionObject| Question object external code |String | cust_REC_Questions| Required
questionObject| Question group object external code |String | cust_REC_QuestionGrouping| Required
stepName| Bot step in the job requisition route map |String | Bot inbox step| Required
outputFolderPath| Folder Path to save bot execution logfile |String | C:\Temp| Optional
logEmail| Email that will receive bot execution logs |String | [sfadminEmail@bestRunSAP.com](mailto:sfadminEmail@bestRunSAP.com)| Optional

Depending on your chosen trigger, bot will automatically trigger for Scheduled triggers or it will be ready to run for Attended triggers.