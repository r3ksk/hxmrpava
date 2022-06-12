The required SuccessFactors configurations to get started with Pre Screen Questions Automation is provided as part of the Store project of **Offer Letter Distribution - SuccessFactors** 

In the previous task you download the automations from the store and downloaded the required configurations files too.

Just follow the SuccessFactors Configurations as per the documentation provided.

Once SAP SuccessFactors Components (API User, Business Rules, MDF Objects and finally sample data) are created. A new job requisition can be posted, candidates can apply and when a candidate is chosen and offer is negotiated, thats when this automation will be useful.

You will be needing the below values at the time of running your automations. so have them handy based on your created sample values. 

>Note:
>Please create sample requisition per your tenant configuration either using Basic Job Requisition template or Standard Job Requisition Template. 


Name | Description | Type | Sample | is it Mandatory?
------------ | ------------ | ------------ | ------------| ------------
apiURL| [API URL of SuccessFactors (see KBA 2215682)](https://userapps.support.sap.com/sap/support/knowledge/en/2215682) |String | [https://apisalesdemo4.successfactors.com:443/odata/v2](https://apisalesdemo4.successfactors.com/odata/v2)| Required
botuser| Bot user username and password |Credential | botuser/password| Required
companyId| CompanyID of the SuccessFactors instance |String | SFTenantName| Required
botStep| Applicant status where candidates will be placed to be picked up by the bot |String | Request Offer Letter| Required
OfferType| Offer type the bot will send. Options are: 1) Online offer (2) Verbal offer (3) Email as text (4) Email as PDF attachment |String | SPA Automation added prescreen questions| Required
sfurl| SuccesFactors application URL |String | [https://salesdemo4.successfactors.com/](https://salesdemo4.successfactors.com/)| Required
