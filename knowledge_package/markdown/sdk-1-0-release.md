SDK 1.0 Release

* [Release Notes](/release-notes/)
* [API](/api/)
* [Types](/types/)
* [Codes](/codes/)
* [Validations](/document-validation-rules/)
* [FAQ](/faq/)
* [Contacts](/contacts/)

SDK 1.0 Release
===============

01 Aug 2025 - Lembaga Hasil Dalam Negeri Malaysia

Lembaga Hasil Dalam Negeri Malaysia has provisioned SDK 1.0 Release to help taxpayers in preparing for the upcoming MyInvois System. SDK Updates section below highlights key updates as part of this release.

Base URLs
=========

In order for taxpayers to access the URLs for the various environments, please ensure that root certificate is trusted by the machine used to avoid any security-related issues accessing these URLs. See more in [FAQ](/faq/#how-to-set-up-environment-to-access-test-apis-and-test-portals).

SDK Updates
===========

**9 August 2025**

**Other Updates**

• With reference to the release note issued on 1 August 2025, which specified the requirement to include the **[Currency Exchange Rate](https://sdk.myinvois.hasil.gov.my/documents/invoice-v1-0/#core)** element when the Invoice Currency Code is not equal to MYR, please be advised of the following timeline:

The validation rule will be applied in the  **Sandbox environment effective 9 August 2025**, and in the  **Production environment effective 1 September 2025**, as previously communicated.

To avoid submission errors, ensure that all e-Invoice payloads involving foreign currency include the **[Currency Exchange Rate](https://sdk.myinvois.hasil.gov.my/documents/invoice-v1-0/#core)** element in compliance with the specified validation rule.

**1 August 2025**

**Updates to API Documentation**

• Added new optional input parameter for Search Taxpayer’s TIN API to enable filtering of
results by entity type (individual or non-individual).

**Other Updates**

• To ensure successful submission, please note that if the **Invoice Currency Code is not equal to MYR**, the payload must include the **[Currency Exchange Rate](https://sdk.myinvois.hasil.gov.my/documents/invoice-v1-0/#core)** element. Submissions will be rejected if **Currency Exchange Rate is missing under these conditions**. Please verify your payload before submission to avoid errors as this validation rule will be **effective from 1 September 2025**.

**4 July 2025**

**Other Updates**

• Added Crimea and Scotland to the list of countries under “Country Codes”  
• Updated Cape Verde to Cabo Verde  
• Removed “(Dutch Part)” from Sint Maarten (Dutch Part)

Changes will be effective from 8 July 2025.

**13 June 2025**

**Updates to API Documentation**

• Updated the maximum number of documents that can be returned by Search Document API to 10,000.

**Other Updates**

• The use of state code ‘00’ is no longer applicable for e-invoice issuance via API / Batch Upload. Please refer to the SDK for the appropriate state codes.

**16 May 2025**

**Other Updates**

• Added new currency code CNH for Yuan Renminbi international trade. The description for code CNY has been amended to differentiate usage for domestic trade.

**28 April 2025**

**Other Updates**

• Kindly take note that data in the sandbox environment will be retained for a maximum of 3 months, after which it will be permanently deleted. Please ensure to back up any important data before the retention period expires.

**25 April 2025**

**Other Updates**

• Please note that the sandbox environment is intended for functional testing and has a lower API rate limit compared to the production environment, effective 28 April 2025.

**11 April 2025**

**Updates to API Documentation**

• Added new API definition for Taxpayer’s QR Code in e-Invoice API section.

**7 February 2025**

**Updates to the XML and JSON samples**

• Added General TIN ‘EI00000000010’ to Consolidated Sample XML and Consolidated Sample JSON.  
• Updated Multi Line Item Sample XML and Multi Line Item Sample JSON with different Tax Type, Tax Rate and Tax Exemption.

**16 January 2025**

**Other Updates**

• The SSL certificate for [myinvois.hasil.gov.my](https://myinvois.hasil.gov.my/) was renewed on 16 January 2025.

**14 January 2025**

**Updates to the API Documentation**

• A rate limit has been added to the [Integration Practices FAQ](https://sdk.myinvois.hasil.gov.my/integration-practices/#rate-limit) section.

**Other Updates**

• Rate limits and important notes have been introduced for the following e-invoice APIs:

* Log in as Taxpayer System
* Log in as Intermediary System
* Submit Documents
* Cancel Document
* Reject Document
* Get Recent Documents
* Get Submission
* Get Document
* Get Document Details
* Search Documents
* Search Taxpayer’s TIN

• We have updated the best practices for optimising API rate limits to ensure optimal performance. The new rate limit will be enforced on May 30, 2025.

**28 December 2024**

**Updates to API Documentation**

• Added new API definition for Search Taxpayers’ TIN in e-Invoice API section.

**Other Updates**

• Added unit code for gross ton (GT) to the system.  
• Updated the sample JSON and XML files for invoice versions 1.0, 1.1 and Signature creation json.

**10 October 2024**

**Updated Validations & Documentation**

• Updated support of Multiline Invoice sample in XML/JSON and the inclusion of MSIC subcategories.

**Updates to API Documentation**

• Removed the Channel parameter in Get Notifications API.  
• Updated Notification Status and Notification Types for Get Notifications.  
• Changed parameter “direction” to “InvoiceDirection”.

**Other Updates**

• Added Netherlands Antilles And Kosovo to list of countries.

**10 August 2024**

**Updates to Signature**

• Included Powershell Script under Signature Creation section for additional guidance on signing JSON file for Version 1.1 document types.

**28 June 2024**

**Updated Validations & Documentation**

• Updated to align API Response and Standard Error Response.  
• Updated the Document Type examples to specify “v1.1” instead of “v1.0”.  
• Removed ‘Continuation Token’ from Search Documents API.

**Updates to Signature**

• Updated detailed step on encoding the hashed property tag using HEX-to-Base64 Encoder in Document Signature Creation.  
• Updated the steps in Signing a JSON Document.

**New Additions**

• Added Signature Page and Relevant Samples for v1.1.  
• Added Type Page and Relevant Samples for v1.1.  
• Added new page (Sample) containing sample payload for each document type.  
• Updated response to the Get All Document Types, Reject Document and Get Recent Documents APIs.

**Other Updates**

• Updated Contacts page.

**21 JUN 2024**

**Updated Validations & Documentation**

• Updated Actual API deployed to Sandbox environment.  
• Updated the UBL Sample XML and JSON for Foreign Currency and Multi Line Item.  
• Added a pagination URL parameter to the Get Submission.  
• Included clarification on Tax Rate.  
• Updated Shipping Recipient fields from “Mandatory where Applicable” to “Optional”.  
• Updated SST Registration Number to a maximum character count of 35 and provided support for the special character – semicolon (;).

**New Additions**

• Implement Minification of XML / JSON documents within the Submit Document API.

**Other Updates**

• Updated the FAQ:

* Added guidance on QR code generation.
* Updated the title from Error 404 to Error 400 and replaced BadArgument with BadRequest.
* Updated TIN parameters.

**24 May 2024**

**Updated Validations & Documentation**

• Amended Number of Characters of Supplier & Buyer Contact Number.  
• Refined note on Tax Rate.  
• Updated Percent node on Tax Rate.

**Updates to Signature**

• Updated sample and explanation of actual Digital Certificate JSON.

**New Additions**

• Added New Sample XML for Foreign Currency with Tax Exchange Rate and Multi Line Item.  
• Added X-Rate Limit Description in FAQ.  
• Added new page for Signing Document JSON in Document Signature Creation page.  
• Added new code ‘E’ under Tax Types.

**Other Updates**

• Included General, Signature and Postman API Guidance subpages under FAQ along with Integration Practices.

**10 May 2024**

**Updated Validations & Documentation**

• Amended descriptions for several fields including Fee / Charge Rate, Fee / Charge Amount, Total Discount Value, and Invoice Additional Fee Amount.  
• Updated available APIs in the sandbox environment under FAQs.  
• Updated cardinality of fields including Quantity, Measurement, Reference Number of Customs Form No.1, 9, etc., SST Registration Number and Tourism Tax Registration Number.  
• Updated number of characters for Measurement field to 3 characters.  
• Refined descriptions for fields such as Tax Type, City Name, Payment Mode, and Prepayment Time.

**Updates to Signature**

• Removal of Timestamp Authority (TSA) requirement of XAdES for digital signature.  
• Provided clearer guidance on hashing with SHA256 followed by HEX-to-Base64 encoding.  
• Updated sample in SDK with RSA-SHA256.

**New Additions**

• Added Measurement Code Table under Codes.

**Other Updates**

• Improved visual for API input parameters with new column on optional / mandatory

**19 April 2024**

**Document Types:**

• Updates to cardinality and number of characters for all document types.  
• Guidance on Taxpayers’ details for MyPR and MyKAS to adhere to NRIC scheme.  
• Updated guidance on address section table.

**e-Invoice API:**

• Updated IdType input parameter to list all possible values.  
• Added new “Mandatory/Optional” column for each API input parameter.

**6 April 2024**

**Updated Validations & Documentation:**

• Updated Types > Invoice v1.0 > All data fields, and Types > Invoice v1.0 > Field descriptions.  
• Updated applicable fields mandatory in Types > Invoice v1.0 > Data Structure.  
• Updated descriptions in Types > Invoice v1.0 > Data Structure.  
• Provided guidance for non-registrants in Types > Invoice v1.0 > Data Structure.  
• Implemented UBL2.1 Sequencing to improve validation and readability.  
• Updated Description field for Fee / Charge Rate.

**New Additions:**

• Added new code ‘044 - Vouchers, gift cards, loyalty points, etc’ in ‘Codes’.  
• Added Tax Exemption Field in Invoice and InvoiceLine.  
• Updated guidance with Digital Signature Creation and Validation, along with sample.

**Updates to API Documentation:**

• Updated API documentation for e-Invoice functionality.  
• Clarified error responses and inputs for various API endpoints.  
• Updated list of Sandbox APIs and Sandbox Identity Service URL on the FAQ page.  
• Updates to writeup of HTTP 400 Error Responses for multiple APIs.

**Other Updates:**

• Improved documentation on document types, hashing, and getting started.  
• Updates to currency exchange rate and file size limitations.  
• Updates to mathematical mapping.

Document Version Updates
========================

Addition of Version 1.1 for all Document Types for Signature Validation.

[Back to homepage](/)