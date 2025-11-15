# Page summaries for https://sdk.myinvois.hasil.gov.my/



---

## Source: https://sdk.myinvois.hasil.gov.my/api/

Application Programming Interface (API) * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Application Programming Interface (API) ======================================= Platform API focuses on key platform functionalities and not dealing with the actual Invoice document. [e-Invoice API](/einvoicingapi/) Login as Taxpayer System ------------------------ This API is used to authenticate the ERP system associated with a specific taxpayer calling and issue access token which allows ERP system to access those protected APIs. [Read more](/api/07-login-as-taxpayer-system/) Login as Intermediary System ---------------------------- This API is used to authenticate the ERP system associated with an intermediary that is representing a taxpayer (acting on behalf of a specific taxpayer) calling and issue access token which allows ERP system to access those protected APIs.



---

## Source: https://sdk.myinvois.hasil.gov.my/api/03-get-document-types/

Get All Document Types * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Get All Document Types ====================== This API allows taxpayer's systems to retrieve list of document types published by the MyInvois System. [Login as Intermediary System](/api/08-login-as-intermediary-system/) [Get Document Type](/api/04-get-document-type/) Overview -------- The main function of the MyInvois System is to enable submission of the issued documents to tax authority. There are multiple types of documents supported by the solution and this API allows taxpayer ERP systems to retrieve their definitions through API call. Signature --------- This is REST based API that does not take additional URL parameters, yet it returns the list of active and deactivated document types that were once active.



---

## Source: https://sdk.myinvois.hasil.gov.my/api/04-get-document-type/

Get Document Type * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Get Document Type ================= This API allows taxpayer's ERP system to retrieve the details of single document type that contains structure definitions of the document. [Get All Document Types](/api/03-get-document-types/) [Get Document Type Version](/api/05-get-document-type-version/) Overview -------- This API allows taxpayer ERP system to retrieve the details of single document type that contains structure definitions of the document. Signature --------- This is REST based API that takes unique ID of the document type as URL parameter and returns document type object with additional details. Signature: `GET /api/v1.0/documenttypes/{id}` Inputs ------ This API accepts [standard e-Invoice API header parameters](/standard-header-parameters/) for authenticated call. | URL parameter |



---

## Source: https://sdk.myinvois.hasil.gov.my/api/05-get-document-type-version/

Get Document Type Version * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Get Document Type Version ========================= This API allows taxpayer's ERP system to retrieve the details of document type version that contains structure definitions of the documents. [Get Document Type](/api/04-get-document-type/) [Get Notifications](/api/06-get-notifications/) Overview -------- This API allows taxpayer ERP system to retrieve the details of document type version that contains structure definitions of the documents that are expected to be submitted as part of [document submission](/einvoicingapi/02-submit-documents/). Document type versions are used to allow document type data fields to be evolved over time without introducing a new document type. For example, if the document type version 1.0 include optional field(s), such field(s) could



---

## Source: https://sdk.myinvois.hasil.gov.my/api/06-get-notifications/

Get Notifications * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Get Notifications ================= This API allows ERP system to query for previously sent notifications. [Get Document Type Version](/api/05-get-document-type-version/) [Full Platform API list](/api/) Overview -------- MyInvois System supports (i) sending out notification via email and (ii) storing the notification in notification history. The ERP system are able to utilise the Get Notification API to query the notification history to obtain the notifications. Note that reliance on notifications for implementing entire e-Invoice workflow is optional and it is provided as an additional functionality that can be leveraged. System limits the number of the notifications that can be received through a single request by implementing paging



---

## Source: https://sdk.myinvois.hasil.gov.my/api/07-login-as-taxpayer-system/

Login as Taxpayer System * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Login as Taxpayer System ======================== This API is used to authenticate the ERP system associated with a specific taxpayer calling and issue access token which allows ERP system to access those protected APIs. [Full Platform API list](/api/) [Login as Intermediary System](/api/08-login-as-intermediary-system/) Overview -------- MyInvois APIs are protected except the Login APIs (Login as taxpayer and Login as Intermediary System) and made available only to relevant taxpayer’s representatives and their ERP systems. This API is used to authenticate the ERP system calling and issue access token which allows ERP system to access those protected APIs. Note that each token issued is issued



---

## Source: https://sdk.myinvois.hasil.gov.my/api/08-login-as-intermediary-system/

Login as Intermediary System * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Login as Intermediary System ============================ This API is used to authenticate the ERP system associated with an intermediary that is representing a taxpayer (acting on behalf of a specific taxpayer) calling and issue access token which allows ERP system to access those protected APIs. [Login as Taxpayer System](/api/07-login-as-taxpayer-system/) [Get All Document Types](/api/03-get-document-types/) Overview -------- MyInvois APIs are protected except the Login APIs (Login as taxpayer and Login as Intermediary System) and made available only to relevant taxpayer’s representatives and their ERP systems. This API is used to authenticate the ERP system calling and issue access token which allows ERP system to



---

## Source: https://sdk.myinvois.hasil.gov.my/codes/

Code Tables * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Code Tables =========== Section contains the definitions of the code tables for reference purposes. Classification Codes -------------------- List of the classification codes and descriptions. [Read more](/codes/classification-codes/) Country Codes ------------- List of country codes allowed as part of the address information as part of the document submission. Country codes are also used for the "Country of Origin" data field. [Read more](/codes/countries/) Currency Codes -------------- List of currency codes allowed as part of the document information during document submission. [Read more](/codes/currencies/) e-Invoice Types --------------- List of e-Invoice types allowed as part of the document submission. [Read more](/codes/e-invoice-types/) Malaysia Standard Industrial Classification (MSIC) Codes -------------------------------------------------------- List



---

## Source: https://sdk.myinvois.hasil.gov.my/codes/classification-codes/

Classification Codes * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Classification Codes ==================== List of the classification codes and descriptions. [Codes](/codes/) Overview ======== Classification code list defines the category of products or services being billed as a result of a commercial transaction. List ==== | Code | Description | | --- | --- | | 001 | Breastfeeding equipment | | 002 | Child care centres and kindergartens fees | | 003 | Computer, smartphone or tablet | | 004 | Consolidated e-Invoice | | 005 | Construction materials (as specified under Fourth Schedule of the Lembaga Pembangunan Industri Pembinaan Malaysia Act 1994) | | 006 | Disbursement | | 007 | Donation



---

## Source: https://sdk.myinvois.hasil.gov.my/codes/countries/

Country Codes * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Country Codes ============= List of country codes allowed as part of the address information as part of the document submission. Country codes are also used for the "Country of Origin" data field. [Codes](/codes/) Overview ======== Country codes are used to supply precise country information when providing address information as part of the document submission. Country codes used in documents are following [ISO-3166 alpha-3 approach](https://www.iso.org/iso-3166-country-codes.html). Country codes are also used for the “Country of Origin” data field. List ==== | Code | Country | | --- | --- | | ABW | ARUBA | | AFG | AFGHANISTAN | | AGO | ANGOLA |



---

## Source: https://sdk.myinvois.hasil.gov.my/codes/currencies/

Currency Codes * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Currency Codes ============== List of currency codes allowed as part of the document information during document submission. [Codes](/codes/) Overview ======== Currency codes are used to supply precise currency information when providing document information as part of the document submission. Currency codes used in documents are following [ISO-4217](https://www.iso.org/iso-4217-currency-codes.html) 3 letter code approach. List ==== | Code | Currency | | --- | --- | | AED | UAE Dirham | | AFN | Afghani | | ALL | Lek | | AMD | Armenian Dram | | ANG | Netherlands Antillean Guilder | | AOA | Kwanza | | ARS | Argentine Peso |



---

## Source: https://sdk.myinvois.hasil.gov.my/codes/e-invoice-types/

e-Invoice Types * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) e-Invoice Types =============== List of e-Invoice types allowed as part of the document submission. [Codes](/codes/) Overview ======== e-Invoice types are used to identify the document type. List ==== | Code | Description | | --- | --- | | 01 | Invoice | | 02 | Credit Note | | 03 | Debit Note | | 04 | Refund Note | | 11 | Self-billed Invoice | | 12 | Self-billed Credit Note | | 13 | Self-billed Debit Note | | 14 | Self-billed Refund Note | File Download ============= [Download JSON file](/files/EInvoiceTypes.json) containing codes of all the e-invoice types. Additional Considerations



---

## Source: https://sdk.myinvois.hasil.gov.my/codes/msic-codes/

Malaysia Standard Industrial Classification (MSIC) Codes * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Malaysia Standard Industrial Classification (MSIC) Codes ======================================================== List of MSIC codes allowed as part of the document and submission. [Codes](/codes/) Overview ======== MSIC codes are 5-digit numeric code that represent the taxpayer’s business nature and activity. MSIC Codes ========== ### BUSINESS CODES | NEW CODES (MSIC 2008) | DESCRIPTION | | --- | --- | | 00000 | NOT APPLICABLE | | **A** | **AGRICULTURE, FORESTRY AND FISHING** | | | CROPS AND ANIMAL PRODUCTION, HUNTING AND RELATED SERVICE ACTIVITIES | | | Growing of non-perennial crops | | 01111 | Growing of maize | | 01112 | Growing



---

## Source: https://sdk.myinvois.hasil.gov.my/codes/payment-methods/

Payment Modes * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Payment Modes ============= Payment Mode refers to the chosen mechanism through which funds are transferred from buyer to supplier. [Codes](/codes/) Overview ======== Payment Mode that may be selected at the time of document submission. List ==== | Code | Description | | --- | --- | | 01 | Cash | | 02 | Cheque | | 03 | Bank Transfer | | 04 | Credit Card | | 05 | Debit Card | | 06 | e-Wallet / Digital Wallet | | 07 | Digital Bank | | 08 | Others | File Download ============= [Download JSON file](/files/PaymentMethods.json) containing codes of all



---

## Source: https://sdk.myinvois.hasil.gov.my/codes/state-codes/

State Codes * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) State Codes =========== List of the state codes representing the names of states and federal territories in Malaysia. [Codes](/codes/) Overview ======== State codes are used to supply precise state information when providing address information as part of the document submission. State codes used in documents are following [ISO-3166](https://www.iso.org/obp/ui/#iso:code:3166:MY). List ==== | Code | State | | --- | --- | | 01 | Johor | | 02 | Kedah | | 03 | Kelantan | | 04 | Melaka | | 05 | Negeri Sembilan | | 06 | Pahang | | 07 | Pulau Pinang | | 08 | Perak | |



---

## Source: https://sdk.myinvois.hasil.gov.my/codes/tax-types/

Tax Types * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Tax Types ========= List of tax types allowed as part of the document and submission. [Codes](/codes/) Overview ======== Tax types are used when entering tax information as part of the invoice (where applicable). List ==== Taxable Types ------------- | Code | Description | | --- | --- | | 01 | Sales Tax | | 02 | Service Tax | | 03 | Tourism Tax | | 04 | High-Value Goods Tax | | 05 | Sales Tax on Low Value Goods | | 06 | Not Applicable | | E | Tax exemption (where applicable) | File Download ============= * [Download JSON



---

## Source: https://sdk.myinvois.hasil.gov.my/codes/unit-types/

Unit of measurement * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Unit of measurement =================== List of unit of measurement types allowed as part of the document line information as part of the document submission. [Codes](/codes/) Overview ======== Unit of measurement types are used as part of the document lines in document submission. This code table is following the UN/ECE Recommendation 20, Revision 17 (2021) as per [here](https://unece.org/trade/documents/revision-17-annexes-i-iii). List ==== Unit Types ---------- | Code | Name | | --- | --- | | 10 | group | | 11 | outfit | | 13 | ration | | 14 | shot | | 15 | stick, military | | 1I | fixed



---

## Source: https://sdk.myinvois.hasil.gov.my/contacts/

Contacts * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Contacts ======== Find LHDNM contact information to reach out in case of any questions regarding MyInvois System and APIs SDK Related Questions ===================== MyInvois Customer Feedback Form: <https://feedback.myinvois.hasil.gov.my> General e-Invoice Questions =========================== E-mail: [myinvois@hasil.gov.my](mailto:myinvois@hasil.gov.my) e-Invoice Microsite: <https://www.hasil.gov.my/en/e-invoice/> Helpdesk Support Hotline ======================== Contact Number : 03 - 8682 8000 [Back to homepage](/)



---

## Source: https://sdk.myinvois.hasil.gov.my/document-validation-rules/

Document validation rules * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Document validation rules ========================= Page describes the validation that is getting applied on every submitted document. Document validation =================== There are different kind of validations that get executed on the submitted document, below is the list of validators that run on submitted documents. 1. Structure Validator 2. Core Fields Validator 3. Signature Validator 4. Taxpayer Validator 5. Referenced Documents Validator 6. Code Validator 7. Duplicate Document Validator 8. Currency Validator Structure Validator ------------------- Validator that enables validation of the submitted document type version to check its structure matching what is required by the document type version. Validator supports validating both [XML](https://docs.oasis-open.org/ubl/UBL-2.1.html) and



---

## Source: https://sdk.myinvois.hasil.gov.my/documents/credit-v1-0/

Credit Note v1.0 * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Credit Note v1.0 ================ v1.0 of the Credit Note document type structure is maintained as v1.1, the only difference is that signature validation is disabled on this version. This version will be deprecated and replaced by version 1.1 at a later date that will be announced later. [Types](/types/) Overview ======== Credit Note is another document type supported by the MyInvois System. It is used to [submit issued invoices](/einvoicingapi/02-submit-documents/) with the Tax Authority. ### Guidance on constructing UBL - In the below Data Structure, if the UBL Schema mapping says / ubl:Invoice / cbc:InvoiceTypeCode / @listVersionID which means that it needs to go



---

## Source: https://sdk.myinvois.hasil.gov.my/documents/credit-v1-1/

Credit Note v1.1 * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Credit Note v1.1 ================ v1.1 of the Credit Note document type structure is maintained as v1.0, the only difference is that signature validation is enabled on this version. [Types](/types/) Overview ======== Credit Note is another document type supported by the MyInvois System. It is used to [submit issued invoices](/einvoicingapi/02-submit-documents/) with the Tax Authority. ### Guidance on constructing UBL - In the below Data Structure, if the UBL Schema mapping says / ubl:Invoice / cbc:InvoiceTypeCode / @listVersionID which means that it needs to go under Invoice element as a InvoiceTypeCode element with an attribute listVersionId. For Example - The UBL XML for InvoiceTypeCode



---

## Source: https://sdk.myinvois.hasil.gov.my/documents/debit-v1-0/

Debit Note v1.0 * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Debit Note v1.0 =============== v1.0 of the Debit Note document type structure is maintained as v1.1, the only difference is that signature validation is disabled on this version. This version will be deprecated and replaced by version 1.1 at a later date that will be announced later. [Types](/types/) Overview ======== Debit Note is another document type supported by the MyInvois System. It is used to [submit issued invoices](/einvoicingapi/02-submit-documents/) with the Tax Authority. ### Guidance on constructing UBL - In the below Data Structure, if the UBL Schema mapping says / ubl:Invoice / cbc:InvoiceTypeCode / @listVersionID which means that it needs to go



---

## Source: https://sdk.myinvois.hasil.gov.my/documents/debit-v1-1/

Debit Note v1.1 * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Debit Note v1.1 =============== v1.1 of the debit Note document type structure is maintained as v1.0, the only difference is that signature validation is enabled on this version. [Types](/types/) Overview ======== Debit Note is another document type supported by the MyInvois System. It is used to [submit issued invoices](/einvoicingapi/02-submit-documents/) with the Tax Authority. ### Guidance on constructing UBL - In the below Data Structure, if the UBL Schema mapping says / ubl:Invoice / cbc:InvoiceTypeCode / @listVersionID which means that it needs to go under Invoice element as a InvoiceTypeCode element with an attribute listVersionId. For Example - The UBL XML for InvoiceTypeCode



---

## Source: https://sdk.myinvois.hasil.gov.my/documents/invoice-v1-0/

Invoice v1.0 * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Invoice v1.0 ============ v1.0 of the Invoice document type structure is maintained as v1.1, the only difference is that signature validation is disabled on this version. This version will be deprecated and replaced by version 1.1 at a later date that will be announced later. [Types](/types/) Overview ======== Invoice is the main document type supported by the MyInvois System. It is used to [submit issued invoices](/einvoicingapi/02-submit-documents/) with the Tax Authority. ### Guidance on constructing UBL - In the below Data Structure, if the UBL Schema mapping says / ubl:Invoice / cbc:InvoiceTypeCode / @listVersionID which means that it needs to go under Invoice element



---

## Source: https://sdk.myinvois.hasil.gov.my/documents/invoice-v1-1/

Invoice v1.1 * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Invoice v1.1 ============ v1.1 of the Invoice document type structure is maintained as v1.0, the only difference is that signature validation is enabled on this version. [Types](/types/) Overview ======== Invoice is the main document type supported by the MyInvois System. It is used to [submit issued invoices](/einvoicingapi/02-submit-documents/) with the Tax Authority. ### Guidance on constructing UBL - In the below Data Structure, if the UBL Schema mapping says / ubl:Invoice / cbc:InvoiceTypeCode / @listVersionID which means that it needs to go under Invoice element as a InvoiceTypeCode element with an attribute listVersionId. For Example - The UBL XML for InvoiceTypeCode will look like



---

## Source: https://sdk.myinvois.hasil.gov.my/documents/refund-v1-0/

Refund Note v1.0 * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Refund Note v1.0 ================ v1.0 of the Refund Note document type structure is maintained as v1.1, the only difference is that signature validation is disabled on this version. This version will be deprecated and replaced by version 1.1 at a later date that will be announced later. [Types](/types/) Overview ======== Refund Note is another document type supported by the MyInvois System. It is used to [submit issued invoices](/einvoicingapi/02-submit-documents/) with the Tax Authority. ### Guidance on constructing UBL - In the below Data Structure, if the UBL Schema mapping says / ubl:Invoice / cbc:InvoiceTypeCode / @listVersionID which means that it needs to go



---

## Source: https://sdk.myinvois.hasil.gov.my/documents/refund-v1-1/

Refund Note v1.1 * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Refund Note v1.1 ================ v1.1 of the refund Note document type structure is maintained as v1.0, the only difference is that signature validation is enabled on this version. [Types](/types/) Overview ======== Refund Note is another document type supported by the MyInvois System. It is used to [submit issued invoices](/einvoicingapi/02-submit-documents/) with the Tax Authority. ### Guidance on constructing UBL - In the below Data Structure, if the UBL Schema mapping says / ubl:Invoice / cbc:InvoiceTypeCode / @listVersionID which means that it needs to go under Invoice element as a InvoiceTypeCode element with an attribute listVersionId. For Example - The UBL XML for InvoiceTypeCode



---

## Source: https://sdk.myinvois.hasil.gov.my/documents/self-billed-credit-v1-0/

Self-Billed Credit Note v1.0 * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Self-Billed Credit Note v1.0 ============================ v1.0 of the Self-Billed Credit Note document type structure is maintained as v1.1, the only difference is that signature validation is disabled on this version. This version will be deprecated and replaced by version 1.1 at a later date that will be announced later. [Types](/types/) Overview ======== Self-billed Credit Note is another document type supported by the MyInvois System. It is used to [submit issued invoices](/einvoicingapi/02-submit-documents/) with the Tax Authority. Note for Self-Billed documents - Supplier (e.g., Foreign Suppliers) could not issue the invoice on MyInvois System. Hence, Buyer issues invoice instead of the supplier. Please



---

## Source: https://sdk.myinvois.hasil.gov.my/documents/self-billed-credit-v1-1/

Self-Billed Credit Note v1.1 * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Self-Billed Credit Note v1.1 ============================ v1.1 of the Self-Billed Credit Note document type structure is maintained as v1.0, the only difference is that signature validation is enabled on this version. [Types](/types/) Overview ======== Self-billed Credit Note is another document type supported by the MyInvois System. It is used to [submit issued invoices](/einvoicingapi/02-submit-documents/) with the Tax Authority. Note for Self-Billed documents - Supplier (e.g., Foreign Suppliers) could not issue the invoice on MyInvois System. Hence, Buyer issues invoice instead of the supplier. Please note that the proper supplier and buyer-related information are being included in the specific invoice. ### Guidance on constructing



---

## Source: https://sdk.myinvois.hasil.gov.my/documents/self-billed-debit-v1-0/

Self-Billed Debit Note v1.0 * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Self-Billed Debit Note v1.0 =========================== v1.0 of the Self-Billed Debit Note document type structure is maintained as v1.1, the only difference is that signature validation is disabled on this version. This version will be deprecated and replaced by version 1.1 at a later date that will be announced later. [Types](/types/) Overview ======== Self-billed Debit Note is the main document type supported by the MyInvois System. It is used to [submit issued invoices](/einvoicingapi/02-submit-documents/) with the Tax Authority. Note for Self-Billed documents - Supplier (e.g., Foreign Suppliers) could not issue the invoice on MyInvois System. Hence, Buyer issues invoice instead of the supplier.



---

## Source: https://sdk.myinvois.hasil.gov.my/documents/self-billed-debit-v1-1/

Self-Billed Debit Note v1.1 * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Self-Billed Debit Note v1.1 =========================== v1.1 of the Self-Billed Debit Note document type structure is maintained as v1.0, the only difference is that signature validation is enabled on this version. [Types](/types/) Overview ======== Self-billed Debit Note is the main document type supported by the MyInvois System. It is used to [submit issued invoices](/einvoicingapi/02-submit-documents/) with the Tax Authority. Note for Self-Billed documents - Supplier (e.g., Foreign Suppliers) could not issue the invoice on MyInvois System. Hence, Buyer issues invoice instead of the supplier. Please note that the proper supplier and buyer-related information are being included in the specific invoice. ### Guidance on



---

## Source: https://sdk.myinvois.hasil.gov.my/documents/self-billed-invoice-v1-0/

Self-Billed Invoice v1.0 * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Self-Billed Invoice v1.0 ======================== v1.0 of the Self-Billed Invoice ddocument type structure is maintained as v1.1, the only difference is that signature validation is disabled on this version. This version will be deprecated and replaced by version 1.1 at a later date that will be announced later. [Types](/types/) Overview ======== Self-billed Invoice is another document type supported by the MyInvois System. It is used to [submit issued invoices](/einvoicingapi/02-submit-documents/) with the Tax Authority. Note for Self-Billed documents - Supplier (e.g., Foreign Suppliers) could not issue the invoice on MyInvois System. Hence, Buyer issues invoice instead of the supplier. Please note that the proper



---

## Source: https://sdk.myinvois.hasil.gov.my/documents/self-billed-invoice-v1-1/

Self-Billed Invoice v1.1 * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Self-Billed Invoice v1.1 ======================== v1.1 of the Self-Billed Invoice document type is the initial version of the Invoices supported by the MyInvois System [Types](/types/) Overview ======== Self-billed Invoice is another document type supported by the MyInvois System. It is used to [submit issued invoices](/einvoicingapi/02-submit-documents/) with the Tax Authority. Note for Self-Billed documents - Supplier (e.g., Foreign Suppliers) could not issue the invoice on MyInvois System. Hence, Buyer issues invoice instead of the supplier. Please note that the proper supplier and buyer-related information are being included in the specific invoice. ### Guidance on constructing UBL - In the below Data Structure, if the



---

## Source: https://sdk.myinvois.hasil.gov.my/documents/self-billed-refund-v1-0/

Self-Billed Refund Note v1.0 * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Self-Billed Refund Note v1.0 ============================ v1.0 of the Self-Billed Refund Note document type structure is maintained as v1.1, the only difference is that signature validation is disabled on this version. This version will be deprecated and replaced by version 1.1 at a later date that will be announced later. [Types](/types/) Overview ======== Self-billed Refund Note is another document type supported by the MyInvois System. It is used to [submit issued invoices](/einvoicingapi/02-submit-documents/) with the Tax Authority. Note for Self-Billed documents - Supplier (e.g., Foreign Suppliers) could not issue the invoice on MyInvois System. Hence, Buyer issues invoice instead of the supplier. Please



---

## Source: https://sdk.myinvois.hasil.gov.my/documents/self-billed-refund-v1-1/

Self-Billed Refund Note v1.1 * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Self-Billed Refund Note v1.1 ============================ v1.1 of the Self-Billed Refund Note document type structure is maintained as v1.0, the only difference is that signature validation is enabled on this version. [Types](/types/) Overview ======== Self-billed Refund Note is another document type supported by the MyInvois System. It is used to [submit issued invoices](/einvoicingapi/02-submit-documents/) with the Tax Authority. Note for Self-Billed documents - Supplier (e.g., Foreign Suppliers) could not issue the invoice on MyInvois System. Hence, Buyer issues invoice instead of the supplier. Please note that the proper supplier and buyer-related information are being included in the specific invoice. ### Guidance on constructing



---

## Source: https://sdk.myinvois.hasil.gov.my/einvoicingapi/

e-Invoice APIs * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) e-Invoice APIs ============== Definition of the API that taxpayer systems can leverage to deal with the actual Invoice documents. [Platform API](/api/) Validate Taxpayer's TIN ----------------------- This API allows taxpayer's ERP system to validate specific Tax Identification Number (TIN) before adding this number to an invoice and issuing the invoice. [Read more](/einvoicingapi/01-validate-taxpayer-tin/) Submit Documents ---------------- This API allows taxpayer to submit one or more signed documents to MyInvois System. [Read more](/einvoicingapi/02-submit-documents/) Cancel Document --------------- This API allows issuer to cancel previously issued document, either self-induced cancellation or by accepting a rejection request made by the buyer. [Read more](/einvoicingapi/03-cancel-document/) Reject Document --------------- This API allows



---

## Source: https://sdk.myinvois.hasil.gov.my/einvoicingapi/01-validate-taxpayer-tin/

Validate Taxpayer's TIN * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Validate Taxpayer's TIN ======================= This API allows taxpayer's ERP system to validate specific Tax Identification Number (TIN) before adding this number to an invoice and issuing the invoice. [Full e-Invoice API list](/einvoicingapi/) [Submit Documents](/einvoicingapi/02-submit-documents/) Overview -------- Validate Taxpayer’s TIN API is used to validate specific Tax Identification Number (TIN) before adding this number to an invoice and issuing the invoice. **Note!** When you are logged in as intermediary, permissions that are granted by the taxpayer will be applied on your profile and this will control the functionalities that you'll be able to executed on behalf of the taxpayer you are representing. Signature



---

## Source: https://sdk.myinvois.hasil.gov.my/einvoicingapi/02-submit-documents/

Submit Documents * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Submit Documents ================ This API allows taxpayer to submit one or more signed documents to MyInvois System. [Validate taxpayer TIN](/einvoicingapi/01-validate-taxpayer-tin/) [Cancel Document](/einvoicingapi/03-cancel-document/) Overview -------- Submit Documents API is the main API of the solution because it is used to submit one or more documents of different types to the system. Documents submitted are grouped into the submission. Then, each document that is part of the submission must be linked to and comply with data structure of the document type (see [document type versions supported](/types/)). Document submission API supports documents submitted using JSON and XML format. Taxpayer ERP system or integration module is responsible



---

## Source: https://sdk.myinvois.hasil.gov.my/einvoicingapi/03-cancel-document/

Cancel Document * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Cancel Document =============== This API allows issuer to cancel previously issued document, either self-induced cancellation or by accepting a rejection request made by the buyer. [Submit Documents](/einvoicingapi/02-submit-documents/) [Reject Document](/einvoicingapi/04-reject-document/) Overview -------- Document cancellation is a way to correct submission errors that were noticed right away. Ideally, cancellation is done even before the document is fully validated and recipient is notified. Therefore, cancellation can be done only within limited time period from the validation of the document. This time limit is specific to document type and is returned by calling [Get Document Type API](/api/04-get-document-type/) and checking workflow parameters. Cancellation is permitted within the 72-hour



---

## Source: https://sdk.myinvois.hasil.gov.my/einvoicingapi/04-reject-document/

Reject Document * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Reject Document =============== This API allows a buyer that received an invoice to reject it and request the supplier to cancel it. [Cancel Document](/einvoicingapi/03-cancel-document/) [Get Recent Documents](/einvoicingapi/05-get-recent-documents/) Overview -------- Document rejection is a way to quickly notify the supplier that there are some problems with the document they have issued, so that correction can be done as soon as possible. Rejection is allowed for recipient of the document only within limited time period from the time of validation of the document. This time limit is specific to document type and is returned by calling [Get Document Type API](/api/04-get-document-type/) and checking workflow parameters. If



---

## Source: https://sdk.myinvois.hasil.gov.my/einvoicingapi/05-get-recent-documents/

Get Recent Documents * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Get Recent Documents ==================== This API allows taxpayer's systems to search the documents sent or received which are available on the MyInvois System using various filters. This API will only return documents that are issued within the last 31 days. [Reject Document](/einvoicingapi/04-reject-document/) [Get Submission](/einvoicingapi/06-get-submission/) Overview -------- Get recent documents API allows users to query the system and return list of documents that have been recently received or issued . System limits the number of the documents that can be received in one request by implementing paging mechanism for this API and also by not allowing to request documents that are issued more



---

## Source: https://sdk.myinvois.hasil.gov.my/einvoicingapi/06-get-submission/

Get Submission * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Get Submission ============== This API returns information on documents submitted during a single submission by taxpayer. [Get Recent Documents](/einvoicingapi/05-get-recent-documents/) [Get Document](/einvoicingapi/07-get-document/) Overview -------- This API allows caller to get details of a single submission to check its processing status after initially [submitting it](/einvoicingapi/02-submit-documents/) and getting back unique submission identifier. This API is available to submitter only as it might contain documents issued to multiple receivers. Signature --------- This is REST based API that takes unique ID of the submission as URL parameter and returns details of the submission and summary information of the documents part of the submission. In view that one submission



---

## Source: https://sdk.myinvois.hasil.gov.my/einvoicingapi/07-get-document/

Get Document * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Get Document ============ This API allows taxpayers to retrieve document source in XML or JSON format along with the additional tax authority metadata. [Get Submission](/einvoicingapi/06-get-submission/) [Get Document Details](/einvoicingapi/08-get-document-details/) Overview -------- This API allows caller to get full details of the document when requested by unique ID assigned to document by MyInvois System. Details include original XML or JSON submission and additional tax authority metadata i.e., additional ID, and current status. As the document is submitted in XML or JSON, this API returns document information also in either XML or JSON. Document with invalid status will not be returned. Details of the invalid document



---

## Source: https://sdk.myinvois.hasil.gov.my/einvoicingapi/08-get-document-details/

Get Document Details * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Get Document Details ==================== This API allows taxpayers to retrieve a single document's full details including validation results. [Get Document](/einvoicingapi/07-get-document/) [Search Documents](/einvoicingapi/09-search-documents/) Overview -------- This API allows caller to get full details of the document when requested by unique ID assigned to document by MyInvois System including the detailed validation results Signature --------- This is REST based API that takes unique ID of the document as URL parameter and returns document details that were received from the issuer and additional details added after registration and validation of the document in the tax authority. Signature: `GET /api/v1.0/documents/{uuid}/details` Rate Limit ---------- To optimize the



---

## Source: https://sdk.myinvois.hasil.gov.my/einvoicingapi/09-search-documents/

Search Documents * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Search Documents ================ This API allows taxpayer's systems to search the documents sent or received which are available on the MyInvois System using various filters. [Get Document Details](/einvoicingapi/08-get-document-details/) [Search Taxpayer's TIN](/einvoicingapi/10-search-taxpayer-tin/) Overview -------- The Search Documents API has various enhanced filters for precise queries and provides access to large result set in a paginated way. Search documents allows users to query the system and return list of documents that have been received or issued. To invoke this API, users must provide values for either the `submissionDateFrom` and `submissionDateTo` filter parameters or the `issueDateFrom` and `issueDateTo` filter parameters. Users can combine these optional filters



---

## Source: https://sdk.myinvois.hasil.gov.my/einvoicingapi/10-search-taxpayer-tin/

Search Taxpayer's TIN * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Search Taxpayer's TIN ===================== This API allows taxpayer's ERP system to search for a specific Tax Identification Number (TIN) using the supported search parameters. The supported search parameters are either: 1) Taxpayer Name or 2) taxpayer, ID Type, ID Value or 3) ID Type, ID Value or 4) ID Type, ID Value, File Type, or 5) If all parameters are provided then the search would use an AND operator to make sure the result found matches all search parameters provided. [Search Documents](/einvoicingapi/09-search-documents/) [Taxpayer's QR Code](/einvoicingapi/11-qr-code/) Overview -------- This API allows taxpayer’s ERP system to search for a specific Tax Identification Number (TIN)



---

## Source: https://sdk.myinvois.hasil.gov.my/einvoicingapi/11-qr-code/

Taxpayer's QR Code * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Taxpayer's QR Code ================== This API allows taxpayer’s ERP system to search and retrieve the information for a specific Taxpayer based on the Base64 formatted string obtained from scanning the respective QR code. [Search Taxpayer's TIN](/einvoicingapi/10-search-taxpayer-tin/) [Full e-Invoice API list](/einvoicingapi/) Overview -------- This API allows taxpayer’s ERP system to retrieve the information for a specific Taxpayer based on the Base64 formatted string obtained from scanning the respective QR code. Signature --------- This is REST based API that searches with Base64 encoded qrCodeText. Signature: GET `/api/v1.0/taxpayers/qrcodeinfo/{qrCodeText}` Rate Limit ---------- To optimize the use of our APIs, a rate limit of 60 Requests Per



---

## Source: https://sdk.myinvois.hasil.gov.my/faq/

Frequently Asked Questions * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Frequently Asked Questions ========================== Answers to frequently asked questions about MyInvois system integration approach [Digital Signature](/signature/) General ======= --- How to retrieve and validate the accuracy of my TIN? ---------------------------------------------------- To facilitate the retrieval of Tax Identification Number (TIN), there are multiple channels available for taxpayers: • Check the TIN via the [MyTax](https://mytax.hasil.gov.my/) Portal (e-Daftar or Your Profile Information). • Validate the TIN via the [Validate Taxpayer’s TIN](https://sdk.myinvois.hasil.gov.my/einvoicingapi/01-validate-taxpayer-tin/) API before submitting e-Invoice. • Contact the HASiL Contact Centre (03-8911 1000); or visit the nearest LHDNM offices. **For Individual TIN (with prefix IG):** • The new prefix for individual TIN is now ‘IG’



---

## Source: https://sdk.myinvois.hasil.gov.my/files/ClassificationCodes.json

[ { "Code": "001", "Description": "Breastfeeding equipment " }, { "Code": "002", "Description": "Child care centres and kindergartens fees" }, { "Code": "003", "Description": "Computer, smartphone or tablet" }, { "Code": "004", "Description": "Consolidated e-Invoice " }, { "Code": "005", "Description": "Construction materials (as specified under Fourth Schedule of the Lembaga Pembangunan Industri Pembinaan Malaysia Act 1994)" }, { "Code": "006", "Description": "Disbursement " }, { "Code": "007", "Description": "Donation" }, { "Code": "008", "Description": "e-Commerce - e-Invoice to buyer / purchaser" }, { "Code": "009", "Description": "e-Commerce - Self-billed e-Invoice to seller, logistics, etc. " }, { "Code": "010", "Description": "Education fees" }, { "Code": "011", "Description": "Goods on consignment (Consignor)" }, { "Code": "012", "Description": "Goods on consignment



---

## Source: https://sdk.myinvois.hasil.gov.my/files/CountryCodes.json

[ { "Code": "ABW", "Country": "ARUBA" }, { "Code": "AFG", "Country": "AFGHANISTAN" }, { "Code": "AGO", "Country": "ANGOLA" }, { "Code": "AIA", "Country": "ANGUILLA" }, { "Code": "ALA", "Country": "ALAND ISLANDS" }, { "Code": "ALB", "Country": "ALBANIA" }, { "Code": "AND", "Country": "ANDORA" }, { "Code": "ANT", "Country": "NETHERLANDS ANTILLE" }, { "Code": "ARE", "Country": "UNITED ARAB EMIRATES" }, { "Code": "ARG", "Country": "ARGENTINA" }, { "Code": "ARM", "Country": "ARMENIA" }, { "Code": "ASM", "Country": "AMERICAN SAMOA" }, { "Code": "ATA", "Country": "ANTARCTICA" }, { "Code": "ATF", "Country": "FRENCH SOUTHERN TERRITORIES" }, { "Code": "ATG", "Country": "ANTIGUA AND BARBUDA" }, { "Code": "AUS", "Country": "AUSTRALIA" }, { "Code": "AUT", "Country": "AUSTRIA" }, { "Code": "AZE", "Country": "AZERBAIDJAN" }, { "Code":



---

## Source: https://sdk.myinvois.hasil.gov.my/files/CurrencyCodes.json

[ { "Code": "AED", "Currency": "UAE Dirham" }, { "Code": "AFN", "Currency": "Afghani" }, { "Code": "ALL", "Currency": "Lek" }, { "Code": "AMD", "Currency": "Armenian Dram" }, { "Code": "ANG", "Currency": "Netherlands Antillean Guilder" }, { "Code": "AOA", "Currency": "Kwanza" }, { "Code": "ARS", "Currency": "Argentine Peso" }, { "Code": "AUD", "Currency": "Australian Dollar" }, { "Code": "AWG", "Currency": "Aruban Florin" }, { "Code": "AZN", "Currency": "Azerbaijan Manat" }, { "Code": "BAM", "Currency": "Convertible Mark" }, { "Code": "BBD", "Currency": "Barbados Dollar" }, { "Code": "BDT", "Currency": "Taka" }, { "Code": "BGN", "Currency": "Bulgarian Lev" }, { "Code": "BHD", "Currency": "Bahraini Dinar" }, { "Code": "BIF", "Currency": "Burundi Franc" }, { "Code": "BMD", "Currency": "Bermudian Dollar" }, { "Code": "BND",



---

## Source: https://sdk.myinvois.hasil.gov.my/files/Digital_Signature_User_Guide.pdf

%PDF-1.7 %µµµµ 1 0 obj <>/Metadata 1601 0 R/ViewerPreferences 1602 0 R>> endobj 2 0 obj <> endobj 3 0 obj <>/ExtGState<>/ProcSet[/PDF/Text/ImageB/ImageC/ImageI] >>/Annots[ 9 0 R 22 0 R] /MediaBox[ 0 0 841.92 595.32] /Contents 4 0 R/Group<>/Tabs/S/StructParents 0>> endobj 4 0 obj <> stream xÝ koIò;ÿaÄ!­gÓ¯y Ý ×%,{+àV&1!±³~pnùïWUýgM<ñ[»ÝSÝU]U]UÝ]=ÜüôÓýç££ ÞÛ öFÁ ·oÅQ ÿ1®dÄA&Yó@å\*<OnßúõÇ`zûÖþëÛ·î?bQ,× oßb  ,\*³H¯/èñI/°\_ ÓïÌý~|ûÖÛÁÉá(T\_B98¿£p(/ ð8ÀÒÓ/B&Ô<²AáðóÁ¯¶î5?B&tõã0/?ÄêgèD¼ÀÏ!g %KÇáI8Lïóp(¿9ÂÞ¼´}@!°NaÿøKÔv¾^?½}ë8öÏÛ·zà°RÀ\Vâ±a­ãhPE > AIÚ¬giË<Þ¶QÍû¦:å ªQWæ(¿ñDºø8³¿/­À jBÅ3(ÍP±NW |9Á&ËÞeÎcd±äë2 3¥°3!¢< dE\* RF" â(Õà ¤­`î?//>OÁ>ü¡!£.TÄ @&d&QÆeÀ(®jýGÉ£8q\*\*ÓV¾0ÂfÐ¨ú©2øÁxÆÚÈBm6Àé$Àê)5VÀV  <; 4~½ MxÝËVDäyJÙAEMÚÅÅeÒI%HP» $Qk ýRR×Ø,G2e@3l 5\_HI!¤ PúùÃ¸DåÐ ð·1èÑÑ!z²Õ^Y¢ âÑÛÓðØ¿D®·Û 0#¿u¯ZýÆvØAïÂ¾ê$yÄ¹U \#áÑ JäZP¿ò¤Vy ]j¦8X¯HòuS<+iÏHýLâ\*Çaù§ª NíøÃ¨]þ¯Âa¢åG?\_âÇ¦·¢N`F¾íä/Îs0k©GTk@ýÌ °r"Ì³u"d¥t´~.)Kvpé  ¾BÁa±i"ÃÂ¿Â!K@¤Ú¿Ò½.Ëí¨Lx²ßR)®J+ËEiìó·Èµ ~Y2$¦\è9A¶ "½ËVk~r5ÍKÑÚ&¨ýJD.UNõós[:&¡ ÷áïYp2/üÄDÈ¤w¥E78[ÌQbT¨«o,3ÌPZ±ýx¡Y^±Ó­Ã-ëñGÚè(Xô¬ÿÅõG2«ÒË'ßáTJ<7ÃÔ¾ ô7ÇY9Öl 4)ÈMi%&@Ê²²O³ÈL î©¾è© ¾\*Ïë¬Fâ K&HaLkN {ÞNõèôX;ôvj á± j wPc{¨ïÄÌSôMÊGKµ÷ÒuZ$Db +Ó\*±ähJkc5IÚÄ¶Óä 5Q´Nj;OªTÕäê@ ªj:b§ AÓN$t´NUë=)KT¥y^Uja" âJ\è¡KH#>dm(Í,ÑPÔ'¥jÕ<îúSä[üó`þ`Yb!Q{².U^ß!jQ¦\ ù¤K QÛ<}¢Ü\9÷ðÐjJ¹KYëÒ ÎÁäª0Õ%±@YÃù$n¬m×4Ö·Å´®ÀõyÖ&+éMr§ üüHNv?ÌþHûj÷ÚdeZtÐååÁ­mf7;UcÚÝØO·YKvÐ+%:lbÜêyH¿WóoåwmjT«âëqQ/Y j³défcÒX­iÝA¹^ ² ÛyÕòÓDo÷Îf!îÄá6 ã¡Tÿ©ÁÄFÍ Õ~ tà¤0A!ü=®. Ôug®oê½Ü8)qÅÏ3ÍK ò4q=Ç;×£1Ë¢LtÑø`jI¸Ú&a (Ð?\*]éi3~ ñá ­¢ÖË èg%=²üü¥ÏØ èZ|¦cQ°}>xðgÈ2 qFí\W\_lÇÚ7÷%¶aR$tâgÒ°\_¡Å­} Åq´wp´÷îàp×a0 ©r#-B~hMÃZH©\*üêPXs#ÕØ#PÓÑ¥SDG3zhBU c,sNã!"ÏNc¿¶³7zÛøNØG³Kô(Ä7ð¦6 ,û,JUM7£zq ©öh¨U÷öÿ\_uoº·ÐÍ3½



---

## Source: https://sdk.myinvois.hasil.gov.my/files/EInvoiceTypes.json

[ { "Code": "01", "Description": "Invoice" }, { "Code": "02", "Description": "Credit Note" }, { "Code": "03", "Description": "Debit Note" }, { "Code": "04", "Description": "Refund Note" }, { "Code": "11", "Description": "Self-billed Invoice" }, { "Code": "12", "Description": "Self-billed Credit Note" }, { "Code": "13", "Description": "Self-billed Debit Note" }, { "Code": "14", "Description": "Self-billed Refund Note" } ]



---

## Source: https://sdk.myinvois.hasil.gov.my/files/MSICSubCategoryCodes.json

[ { "Code": "00000", "Description": "NOT APPLICABLE", "MSIC Category Reference": "" }, { "Code": "01111", "Description": "Growing of maize", "MSIC Category Reference": "A" }, { "Code": "01112", "Description": "Growing of leguminous crops", "MSIC Category Reference": "A" }, { "Code": "01113", "Description": "Growing of oil seeds", "MSIC Category Reference": "A" }, { "Code": "01119", "Description": "Growing of other cereals n.e.c.", "MSIC Category Reference": "A" }, { "Code": "01120", "Description": "Growing of paddy", "MSIC Category Reference": "A" }, { "Code": "01131", "Description": "Growing of leafy or stem vegetables", "MSIC Category Reference": "A" }, { "Code": "01132", "Description": "Growing of fruits bearing vegetables", "MSIC Category Reference": "A" }, { "Code": "01133", "Description": "Growing of melons", "MSIC Category Reference": "A" }, { "Code": "01134",



---

## Source: https://sdk.myinvois.hasil.gov.my/files/PaymentMethods.json

[ { "Code": "01", "Payment Method": "Cash" }, { "Code": "02", "Payment Method": "Cheque" }, { "Code": "03", "Payment Method": "Bank Transfer" }, { "Code": "04", "Payment Method": "Credit Card" }, { "Code": "05", "Payment Method": "Debit Card" }, { "Code": "06", "Payment Method": "e-Wallet / Digital Wallet" }, { "Code": "07", "Payment Method": "Digital Bank" }, { "Code": "08", "Payment Method": "Others" } ]



---

## Source: https://sdk.myinvois.hasil.gov.my/files/StateCodes.json

[ { "Code": "01", "State": "Johor" }, { "Code": "02", "State": "Kedah" }, { "Code": "03", "State": "Kelantan" }, { "Code": "04", "State": "Melaka" }, { "Code": "05", "State": "Negeri Sembilan" }, { "Code": "06", "State": "Pahang" }, { "Code": "07", "State": "Pulau Pinang" }, { "Code": "08", "State": "Perak" }, { "Code": "09", "State": "Perlis" }, { "Code": "10", "State": "Selangor" }, { "Code": "11", "State": "Terengganu" }, { "Code": "12", "State": "Sabah" }, { "Code": "13", "State": "Sarawak" }, { "Code": "14", "State": "Wilayah Persekutuan Kuala Lumpur" }, { "Code": "15", "State": "Wilayah Persekutuan Labuan" }, { "Code": "16", "State": "Wilayah Persekutuan Putrajaya" }, { "Code": "17", "State": "Not Applicable" } ]



---

## Source: https://sdk.myinvois.hasil.gov.my/files/TaxTypes.json

[ { "Code": "01", "Description": "Sales Tax" }, { "Code": "02", "Description": "Service Tax" }, { "Code": "03", "Description": "Tourism Tax" }, { "Code": "04", "Description": "High-Value Goods Tax" }, { "Code": "05", "Description": "Sales Tax on Low Value Goods" }, { "Code": "06", "Description": "Not Applicable" }, { "Code": "E", "Description": "Tax exemption (where applicable)" } ]



---

## Source: https://sdk.myinvois.hasil.gov.my/files/UnitTypes.json

[ { "Code": "10", "Name": "group" }, { "Code": "11", "Name": "outfit" }, { "Code": "13", "Name": "ration" }, { "Code": "14", "Name": "shot" }, { "Code": "15", "Name": "stick, military" }, { "Code": "1I", "Name": "fixed rate" }, { "Code": "20", "Name": "twenty foot container" }, { "Code": "21", "Name": "forty foot container" }, { "Code": "22", "Name": "decilitre per gram" }, { "Code": "23", "Name": "gram per cubic centimetre" }, { "Code": "24", "Name": "theoretical pound" }, { "Code": "25", "Name": "gram per square centimetre" }, { "Code": "27", "Name": "theoretical ton" }, { "Code": "28", "Name": "kilogram per square metre" }, { "Code": "2A", "Name": "radian per second" }, { "Code": "2B", "Name": "radian per second squared"



---

## Source: https://sdk.myinvois.hasil.gov.my/files/one-doc-signed.xml

urn:oasis:names:specification:ubl:dsig:enveloped:xades urn:oasis:names:specification:ubl:signature:1 urn:oasis:names:specification:ubl:signature:Invoice not(//ancestor-or-self::ext:UBLExtensions) not(//ancestor-or-self::cac:Signature) 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 2024-07-23T16:31:06Z KKBSTyiPKGkGl1AFqcPziKCEIDYGtnYUTQN4ukO7G40= CN=Trial LHDNM Sub CA V1, OU=Terms of use at http://www.posdigicert.com.my, O=LHDNM, C=MY 162880276254639189035871514749820882117 XML-INV12345 2024-07-23 00:40:00Z 01 MYR MYR 2024-07-01 2024-07-31 Monthly 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 urn:oasis:names:specification:ubl:signature:Invoice urn:oasis:names:specification:ubl:dsig:enveloped:xades CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method is cash E12345678912 1.00 2024-07-23



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sample-ul-invoice-2.1-signed.min.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-INV12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "01", "listVersionID": "1.1" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] } ], "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ], "DocumentType": [ { "\_": "CustomsImportForm" } ] }, { "ID": [ { "\_":



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Credit-Note-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-CN12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "02", "listVersionID": "1.0" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "InvoiceDocumentReference": [ { "ID": [ { "\_": "JSON-INV12345" } ], "UUID": [ { "\_": "Reference Invoice UUID" } ] } ] }, { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] } ],



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Credit-Note-Sample.xml

XML-CN12345 2024-07-23 00:40:00Z 02 MYR MYR 2024-07-01 2024-07-31 Monthly XML-INV12345 Reference Invoice UUID 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method is cash E12345678912 1.00 2024-07-23 00:30:00Z false Sample Description 100 true Service charge 100 87.63 87.63 87.63 01 OTH 1436.50 1436.50 1436.50 1436.50 1436.50 0.30 1436.50 1234



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Debit-Note-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-DN12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "03", "listVersionID": "1.0" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "InvoiceDocumentReference": [ { "ID": [ { "\_": "JSON-INV12345" } ], "UUID": [ { "\_": "Reference Invoice UUID" } ] } ] }, { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] } ],



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Debit-Note-Sample.xml

XML-DN12345 2024-07-23 00:40:00Z 03 MYR MYR 2024-07-01 2024-07-31 Monthly XML-INV12345 Reference Invoice UUID 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method is cash E12345678912 1.00 2024-07-23 00:30:00Z false Sample Description 100 true Service charge 100 87.63 87.63 87.63 01 OTH 1436.50 1436.50 1436.50 1436.50 1436.50 0.30 1436.50 1234



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Invoice-Consolidated-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-INV12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "01", "listVersionID": "1.0" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "AccountingSupplierParty": [ { "Party": [ { "IndustryClassificationCode": [ { "\_": "46510", "name": "Wholesale of computer hardware, software and peripherals" } ], "PartyIdentification": [ { "ID": [ { "\_": "Supplier's TIN", "schemeID": "TIN" } ] }, { "ID": [ { "\_": "Supplier's BRN", "schemeID": "BRN" } ] }, { "ID": [ { "\_": "NA", "schemeID": "SST" } ] }, { "ID": [ { "\_": "NA", "schemeID": "TTX"



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Invoice-Consolidated-Sample.xml

XML-INV12345 2024-07-23 00:40:00Z 01 MYR MYR 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com EI00000000010 NA NA NA NA Consolidated Buyers NA NA 3000 30000 3000 01 OTH 30000 30000 33000 0 0 0 33000 1 1 10000 1000 10000 1000 10.00 01 OTH Receipt 001 - 100 MYS 004 10000 10000 2 1 20000 2000 20000 2000 10.00 01 OTH Receipt 101 - 200 MYS 004 20000 20000



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Invoice-ForeignCurrency-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-INV12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "01", "listVersionID": "1.0" } ], "DocumentCurrencyCode": [ { "\_": "USD" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] } ], "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ], "DocumentType": [ { "\_": "CustomsImportForm" } ] }, { "ID": [ { "\_":



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Invoice-ForeignCurrency-Sample.xml

XML-INV12345 2024-07-23 00:40:00Z 01 USD MYR 2024-07-01 2024-07-31 Monthly 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method is cash E12345678912 1.00 2024-07-23 00:30:00Z false Sample Description 100 true Service charge 100 USD MYR 4.72 87.63 87.63 87.63 01 OTH 1436.50 1436.50 1436.50 1436.50 1436.50 0.30 1436.50 1234 1



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Invoice-MultiLineItem-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-INV12345" } ], "IssueDate": [ { "\_": "2025-02-06" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "01", "listVersionID": "1.0" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2025-01-01" } ], "EndDate": [ { "\_": "2025-01-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] } ], "AdditionalDocumentReference": [ { "ID": [ { "\_": "E23456789123,E98765432123" } ], "DocumentType": [ { "\_": "CustomsImportForm" } ] }, { "ID": [ { "\_":



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Invoice-MultiLineItem-Sample.xml

XML-INV12345 2025-02-06 00:30:00Z 01 MYR MYR 2025-01-01 2025-01-31 Monthly E12345678912 E23456789123,E98765432123 CustomsImportForm FTA FreeTradeAgreement ASEAN-Australia-New Zealand FTA (AANZFTA) E12345678912,E23456789123 K2 CIF CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com false 0.00 true 0.00 85.00 1000.00 10.00 01 OTH 1500.00 75.00 02 OTH 2000.00 100.00 E OTH 4500.00 4500.00 4585.00 0.00 0.00 0.00 4585.00 001 1 1000.00 false 0 0.00 true 0 0.00 10.00 1000.00 10.00 1 10.00 01 OTH Laptop Peripherals MYS 9800.00.0010 003 1000.00 1000.00 002 1 1500.00 false 0 0.00 true 0



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Invoice-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-INV12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "01", "listVersionID": "1.0" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] } ], "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ], "DocumentType": [ { "\_": "CustomsImportForm" } ] }, { "ID": [ { "\_":



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Invoice-Sample.xml

XML-INV12345 2024-07-23 00:40:00Z 01 MYR MYR 2024-07-01 2024-07-31 Monthly 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method is cash E12345678912 1.00 2024-07-23 00:30:00Z false Sample Description 100 true Service charge 100 87.63 87.63 87.63 01 OTH 1436.50 1436.50 1436.50 1436.50 1436.50 0.30 1436.50 1234 1 1436.50 false Sample



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Refund-Note-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-RN12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "04", "listVersionID": "1.0" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "InvoiceDocumentReference": [ { "ID": [ { "\_": "JSON-INV12345" } ], "UUID": [ { "\_": "Reference Invoice UUID" } ] } ] }, { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] } ],



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Refund-Note-Sample.xml

XML-RN12345 2024-07-23 00:40:00Z 04 MYR MYR 2024-07-01 2024-07-31 Monthly XML-INV12345 Reference Invoice UUID 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method is cash E12345678912 1.00 2024-07-23 00:30:00Z false Sample Description 100 true Service charge 100 87.63 87.63 87.63 01 OTH 1436.50 1436.50 1436.50 1436.50 1436.50 0.30 1436.50 1234



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Self-Billed-Credit-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-SBCN12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "12", "listVersionID": "1.0" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "InvoiceDocumentReference": [ { "ID": [ { "\_": "JSON-SBINV12345" } ], "UUID": [ { "\_": "Reference Self-billed Invoice UUID" } ] } ] }, { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] }



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Self-Billed-Credit-Sample.xml

XML-SBCN12345 2024-07-23 00:40:00Z 12 MYR MYR 2024-07-01 2024-07-31 Monthly XML-SBINV12345 Reference Self-billed Invoice UUID 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method is cash E12345678912 1.00 2024-07-23 00:30:00Z false Sample Description 100 true Service charge 100 87.63 87.63 87.63 01 OTH 1436.50 1436.50 1436.50 1436.50 1436.50 0.30 1436.50



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Self-Billed-Debit-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-SBDN12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "13", "listVersionID": "1.0" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "InvoiceDocumentReference": [ { "ID": [ { "\_": "JSON-SBINV12345" } ], "UUID": [ { "\_": "Reference Self-billed Invoice UUID" } ] } ] }, { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] }



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Self-Billed-Debit-Sample.xml

XML-SBDN12345 2024-07-23 00:40:00Z 13 MYR MYR 2024-07-01 2024-07-31 Monthly XML-SBINV12345 Reference Self-billed Invoice UUID 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method is cash E12345678912 1.00 2024-07-23 00:30:00Z false Sample Description 100 true Service charge 100 87.63 87.63 87.63 01 OTH 1436.50 1436.50 1436.50 1436.50 1436.50 0.30 1436.50



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Self-Billed-Invoice-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-SBINV12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "11", "listVersionID": "1.0" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] } ], "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ], "DocumentType": [ { "\_": "CustomsImportForm" } ] }, { "ID": [ { "\_":



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Self-Billed-Invoice-Sample.xml

XML-SBINV12345 2024-07-23 00:40:00Z 11 MYR MYR 2024-07-01 2024-07-31 Monthly 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method is cash E12345678912 1.00 2024-07-23 00:30:00Z false Sample Description 100 true Service charge 100 87.63 87.63 87.63 01 OTH 1436.50 1436.50 1436.50 1436.50 1436.50 0.30 1436.50 1234 1 1436.50 false Sample



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Self-Billed-Refund-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-SBRN12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "14", "listVersionID": "1.0" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "InvoiceDocumentReference": [ { "ID": [ { "\_": "JSON-SBINV12345" } ], "UUID": [ { "\_": "Reference Self-billed Invoice UUID" } ] } ] }, { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] }



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.0-Self-Billed-Refund-Sample.xml

XML-SBRN12345 2024-07-23 00:40:00Z 14 MYR MYR 2024-07-01 2024-07-31 Monthly XML-SBINV12345 Reference Self-billed Invoice UUID 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method is cash E12345678912 1.00 2024-07-23 00:30:00Z false Sample Description 100 true Service charge 100 87.63 87.63 87.63 01 OTH 1436.50 1436.50 1436.50 1436.50 1436.50 0.30 1436.50



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Credit-Note-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-CN12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "02", "listVersionID": "1.1" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "InvoiceDocumentReference": [ { "ID": [ { "\_": "JSON-INV12345" } ], "UUID": [ { "\_": "Reference Invoice UUID" } ] } ] }, { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] } ],



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Credit-Note-Sample.xml

urn:oasis:names:specification:ubl:dsig:enveloped:xades urn:oasis:names:specification:ubl:signature:1 urn:oasis:names:specification:ubl:signature:Invoice not(//ancestor-or-self::ext:UBLExtensions) not(//ancestor-or-self::cac:Signature) 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 2024-07-23T18:01:59Z KKBSTyiPKGkGl1AFqcPziKCEIDYGtnYUTQN4ukO7G40= CN=Trial LHDNM Sub CA V1, OU=Terms of use at http://www.posdigicert.com.my, O=LHDNM, C=MY 162880276254639189035871514749820882117 XML-CN12345 2024-07-23 00:40:00Z 02 MYR MYR 2024-07-01 2024-07-31 Monthly XML-INV12345 Reference Invoice UUID 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 urn:oasis:names:specification:ubl:signature:Invoice urn:oasis:names:specification:ubl:dsig:enveloped:xades CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method is



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Debit-Note-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-DN12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "03", "listVersionID": "1.1" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "InvoiceDocumentReference": [ { "ID": [ { "\_": "JSON-INV12345" } ], "UUID": [ { "\_": "Reference Invoice UUID" } ] } ] }, { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] } ],



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Debit-Note-Sample.xml

urn:oasis:names:specification:ubl:dsig:enveloped:xades urn:oasis:names:specification:ubl:signature:1 urn:oasis:names:specification:ubl:signature:Invoice not(//ancestor-or-self::ext:UBLExtensions) not(//ancestor-or-self::cac:Signature) 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 2024-07-23T18:07:17Z KKBSTyiPKGkGl1AFqcPziKCEIDYGtnYUTQN4ukO7G40= CN=Trial LHDNM Sub CA V1, OU=Terms of use at http://www.posdigicert.com.my, O=LHDNM, C=MY 162880276254639189035871514749820882117 XML-DN12345 2024-07-23 00:40:00Z 03 MYR MYR 2024-07-01 2024-07-31 Monthly XML-INV12345 Reference Invoice UUID 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 urn:oasis:names:specification:ubl:signature:Invoice urn:oasis:names:specification:ubl:dsig:enveloped:xades CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method is



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Invoice-Consolidated-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-INV12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "01", "listVersionID": "1.1" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "AccountingSupplierParty": [ { "Party": [ { "IndustryClassificationCode": [ { "\_": "46510", "name": "Wholesale of computer hardware, software and peripherals" } ], "PartyIdentification": [ { "ID": [ { "\_": "Supplier's TIN", "schemeID": "TIN" } ] }, { "ID": [ { "\_": "Supplier's BRN", "schemeID": "BRN" } ] }, { "ID": [ { "\_": "NA", "schemeID": "SST" } ] }, { "ID": [ { "\_": "NA", "schemeID": "TTX"



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Invoice-Consolidated-Sample.xml

urn:oasis:names:specification:ubl:dsig:enveloped:xades urn:oasis:names:specification:ubl:signature:1 urn:oasis:names:specification:ubl:signature:Invoice not(//ancestor-or-self::ext:UBLExtensions) not(//ancestor-or-self::cac:Signature) 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 2025-02-05T07:43:54Z KKBSTyiPKGkGl1AFqcPziKCEIDYGtnYUTQN4ukO7G40= CN=Trial LHDNM Sub CA V1, OU=Terms of use at http://www.posdigicert.com.my, O=LHDNM, C=MY 162880276254639189035871514749820882117 XML-INV12345 2024-07-23 00:40:00Z 01 MYR MYR urn:oasis:names:specification:ubl:signature:Invoice urn:oasis:names:specification:ubl:dsig:enveloped:xades 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com EI00000000010 NA NA NA NA Consolidated Buyers NA NA 3000 30000 3000 01 OTH 30000 30000 33000 0 0 0 33000 1 1 10000 1000 10000 1000 10.00 01 OTH Receipt 001 - 100 MYS 004 10000 10000 2 1 20000 2000 20000 2000 10.00 01 OTH Receipt 101 - 200 MYS 004 20000 20000



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Invoice-ForeignCurrency-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-INV12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "01", "listVersionID": "1.1" } ], "DocumentCurrencyCode": [ { "\_": "USD" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] } ], "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ], "DocumentType": [ { "\_": "CustomsImportForm" } ] }, { "ID": [ { "\_":



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Invoice-ForeignCurrency-Sample.xml

urn:oasis:names:specification:ubl:dsig:enveloped:xades urn:oasis:names:specification:ubl:signature:1 urn:oasis:names:specification:ubl:signature:Invoice not(//ancestor-or-self::ext:UBLExtensions) not(//ancestor-or-self::cac:Signature) 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 2024-07-23T00:30:05Z ZCNpyqI3UdD9J2vYgzH7gwkR0IcQjkjhB4Lb0rgC3jQ= CN=Trial LHDNM Sub CA V1, OU=Terms of use at http://www.posdigicert.com.my, O=LHDNM, C=MY 474536 XML-INV12345 2024-07-23 00:30:00Z 01 USD MYS 2024-07-01 2024-07-31 Monthly 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 urn:oasis:names:specification:ubl:signature:Invoice urn:oasis:names:specification:ubl:dsig:enveloped:xades CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method is cash E12345678912 1.00 2024-07-23



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Invoice-MultiLineItem-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-INV12345" } ], "IssueDate": [ { "\_": "2025-02-06" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "01", "listVersionID": "1.1" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2025-01-01" } ], "EndDate": [ { "\_": "2025-01-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] } ], "AdditionalDocumentReference": [ { "ID": [ { "\_": "E23456789123,E98765432123" } ], "DocumentType": [ { "\_": "CustomsImportForm" } ] }, { "ID": [ { "\_":



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Invoice-MultiLineItem-Sample.xml

urn:oasis:names:specification:ubl:dsig:enveloped:xades urn:oasis:names:specification:ubl:signature:1 urn:oasis:names:specification:ubl:signature:Invoice not(//ancestor-or-self::ext:UBLExtensions) not(//ancestor-or-self::cac:Signature) 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 2025-04-15T02:00:22Z +kdLjFra9qRhG35bEKff9ZPjj6Bq6W6/j0NS0st/ves= C=MY, O=Raffcomm Technologies Sdn Bhd, OU=1000449-W, CN=CypherSign Pro Max 1308502606566147853 XML-INV12345 2025-02-06 00:30:00Z 01 MYR MYR 2025-01-01 2025-01-31 Monthly E12345678912 E23456789123,E98765432123 CustomsImportForm FTA FreeTradeAgreement ASEAN-Australia-New Zealand FTA (AANZFTA) E12345678912,E23456789123 K2 CIF urn:oasis:names:specification:ubl:signature:Invoice urn:oasis:names:specification:ubl:dsig:enveloped:xades CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com false 0.00 true 0.00 85.00 1000.00 10.00 01 OTH 1500.00 75.00 02 OTH 2000.00 100.00 E OTH 4500.00 4500.00 4585.00 0.00 0.00 0.00 4585.00 001 1 1000.00 false 0 0.00 true 0



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Invoice-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-INV12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "01", "listVersionID": "1.1" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] } ], "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ], "DocumentType": [ { "\_": "CustomsImportForm" } ] }, { "ID": [ { "\_":



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Invoice-Sample.xml

urn:oasis:names:specification:ubl:dsig:enveloped:xades urn:oasis:names:specification:ubl:signature:1 urn:oasis:names:specification:ubl:signature:Invoice not(//ancestor-or-self::ext:UBLExtensions) not(//ancestor-or-self::cac:Signature) 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 2024-07-23T16:31:06Z KKBSTyiPKGkGl1AFqcPziKCEIDYGtnYUTQN4ukO7G40= CN=Trial LHDNM Sub CA V1, OU=Terms of use at http://www.posdigicert.com.my, O=LHDNM, C=MY 162880276254639189035871514749820882117 XML-INV12345 2024-07-23 00:40:00Z 01 MYR MYR 2024-07-01 2024-07-31 Monthly 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 urn:oasis:names:specification:ubl:signature:Invoice urn:oasis:names:specification:ubl:dsig:enveloped:xades CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method is cash E12345678912 1.00 2024-07-23



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Refund-Note-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-RN12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "04", "listVersionID": "1.1" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "InvoiceDocumentReference": [ { "ID": [ { "\_": "JSON-INV12345" } ], "UUID": [ { "\_": "Reference Invoice UUID" } ] } ] }, { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] } ],



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Refund-Note-Sample.xml

urn:oasis:names:specification:ubl:dsig:enveloped:xades urn:oasis:names:specification:ubl:signature:1 urn:oasis:names:specification:ubl:signature:Invoice not(//ancestor-or-self::ext:UBLExtensions) not(//ancestor-or-self::cac:Signature) 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 2024-07-23T18:08:30Z KKBSTyiPKGkGl1AFqcPziKCEIDYGtnYUTQN4ukO7G40= CN=Trial LHDNM Sub CA V1, OU=Terms of use at http://www.posdigicert.com.my, O=LHDNM, C=MY 162880276254639189035871514749820882117 XML-RN12345 2024-07-23 00:40:00Z 04 MYR MYR 2024-07-01 2024-07-31 Monthly XML-INV12345 Reference Invoice UUID 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 urn:oasis:names:specification:ubl:signature:Invoice urn:oasis:names:specification:ubl:dsig:enveloped:xades CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method is



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Self-Billed-Credit-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-SBCN12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "12", "listVersionID": "1.1" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "InvoiceDocumentReference": [ { "ID": [ { "\_": "JSON-SBINV12345" } ], "UUID": [ { "\_": "Reference Self-billed Invoice UUID" } ] } ] }, { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] }



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Self-Billed-Credit-Sample.xml

urn:oasis:names:specification:ubl:dsig:enveloped:xades urn:oasis:names:specification:ubl:signature:1 urn:oasis:names:specification:ubl:signature:Invoice not(//ancestor-or-self::ext:UBLExtensions) not(//ancestor-or-self::cac:Signature) +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 2024-07-23T18:50:34Z KKBSTyiPKGkGl1AFqcPziKCEIDYGtnYUTQN4ukO7G40= CN=Trial LHDNM Sub CA V1, OU=Terms of use at http://www.posdigicert.com.my, O=LHDNM, C=MY 162880276254639189035871514749820882117 XML-SBCN12345 2024-07-23 00:40:00Z 12 MYR MYR 2024-07-01 2024-07-31 Monthly XML-SBINV12345 Reference Self-billed Invoice UUID 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 urn:oasis:names:specification:ubl:signature:Invoice urn:oasis:names:specification:ubl:dsig:enveloped:xades CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Self-Billed-Debit-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-SBDN12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "13", "listVersionID": "1.1" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "InvoiceDocumentReference": [ { "ID": [ { "\_": "JSON-SBINV12345" } ], "UUID": [ { "\_": "Reference Self-billed Invoice UUID" } ] } ] }, { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] }



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Self-Billed-Debit-Sample.xml

urn:oasis:names:specification:ubl:dsig:enveloped:xades urn:oasis:names:specification:ubl:signature:1 urn:oasis:names:specification:ubl:signature:Invoice not(//ancestor-or-self::ext:UBLExtensions) not(//ancestor-or-self::cac:Signature) zc2mfZLdPL6UXMfIf8miiuKuUpbMc9NKvdRYDHFTDa0= oJFMR/hwRkcJ2rygRaH35bpKcyx/d1S9Mszb8av0aWY= VIjLKomk4wa4hInxPqVEkf94SdTCnCefyV3AHbKyzzO6H4RFT35kCozx0fLqX5PkdsJftFjR/3+K27u3v0M3yS3oOOtiwl/Y4E+Q2cbSDKnpEsFgxWBWeN85mhJ3v8IeLwmepQ9/XpqPryu+vwzILvnjHVvBRNLlsHqlx5ohfqayU+McuoSzGkFkQWtnoX/TUNtFjdUo1096tRNmLrA+3DiFaQyrO/sVgEZu8bevOXUeLZTmPDyZDz41N0SQB+Bx5zNwCQXLCtZhWXasBvFtU1kofviN6BzZocDquWYi5ZXirkTWJKtb5cifD4HWs8FFRnW2f56cMQEQWFOVdS0Drw== MIIFlDCCA3ygAwIBAgIQeomZorO+0AwmW2BRdWJMxTANBgkqhkiG9w0BAQsFADB1MQswCQYDVQQGEwJNWTEOMAwGA1UEChMFTEhETk0xNjA0BgNVBAsTLVRlcm1zIG9mIHVzZSBhdCBodHRwOi8vd3d3LnBvc2RpZ2ljZXJ0LmNvbS5teTEeMBwGA1UEAxMVVHJpYWwgTEhETk0gU3ViIENBIFYxMB4XDTI0MDYwNjAyNTIzNloXDTI0MDkwNjAyNTIzNlowgZwxCzAJBgNVBAYTAk1ZMQ4wDAYDVQQKEwVEdW1teTEVMBMGA1UEYRMMQzI5NzAyNjM1MDYwMRswGQYDVQQLExJUZXN0IFVuaXQgZUludm9pY2UxDjAMBgNVBAMTBUR1bW15MRIwEAYDVQQFEwlEMTIzNDU2NzgxJTAjBgkqhkiG9w0BCQEWFmFuYXMuYUBmZ3Zob2xkaW5ncy5jb20wggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQChvfOzAofnU60xFO7NcmF2WRi+dgor1D7ccISgRVfZC30Fdxnt1S6ZNf78Lbrz8TbWMicS8plh/pHy96OJvEBplsAgcZTd6WvaMUB2oInC86D3YShlthR6EzhwXgBmg/g9xprwlRqXMT2p4+K8zmyJZ9pIb8Y+tQNjm/uYNudtwGVm8A4hEhlRHbgfUXRzT19QZml6V2Ea0wQI8VyWWa8phCIkBD2w4F8jG4eP5/0XSQkTfBHHf+GV/YDJx5KiiYfmB1nGfwoPHix6Gey+wRjIq87on8Dm5+8ei8/bOhcuuSlpxgwphAP3rZrNbRN9LNVLSQ5md41asoBHfaDIVPVpAgMBAAGjgfcwgfQwHwYDVR0lBBgwFgYIKwYBBQUHAwQGCisGAQQBgjcKAwwwEQYDVR0OBAoECEDwms66hrpiMFMGA1UdIARMMEowSAYJKwYBBAGDikUBMDswOQYIKwYBBQUHAgEWLWh0dHBzOi8vd3d3LnBvc2RpZ2ljZXJ0LmNvbS5teS9yZXBvc2l0b3J5L2NwczATBgNVHSMEDDAKgAhNf9lrtsUI0DAOBgNVHQ8BAf8EBAMCBkAwRAYDVR0fBD0wOzA5oDegNYYzaHR0cDovL3RyaWFsY3JsLnBvc2RpZ2ljZXJ0LmNvbS5teS9UcmlhbExIRE5NVjEuY3JsMA0GCSqGSIb3DQEBCwUAA4ICAQBwptnIb1OA8NNVotgVIjOnpQtowew87Y0EBWAnVhOsMDlWXD/s+BL7vIEbX/BYa0TjakQ7qo4riSHyUkQ+X+pNsPEqolC4uFOp0pDsIdjsNB+WG15itnghkI99c6YZmbXcSFw9E160c7vG25gIL6zBPculHx5+laE59YkmDLdxx27e0TltUbFmuq3diYBOOf7NswFcDXCo+kXOwFfgmpbzYS0qfSoh3eZZtVHg0r6uga1UsMGb90+IRsk4st99EOVENvo0290lWhPBVK2G34+2TzbbYnVkoxnq6uDMw3cRpXX/oSfya+tyF51kT3iXvpmQ9OMF3wMlfKwCS7BZB2+iRja/1WHkAP7QW7/+0zRBcGQzY7AYsdZUllwYapsLEtbZBrTiH12X4XnZjny9rLfQLzJsFGT7Q+e02GiCsBrK7ZHNTindLRnJYAo4U2at5+SjqBiXSmz0DG+juOyFkwiWyD0xeheg4tMMO2pZ7clQzKflYnvFTEFnt+d+tvVwNjTboxfVxEv2qWF6qcMJeMvXwKTXuwVI2iUqmJSzJbUY+w3OeG7fvrhUfMJPM9XZBOp7CEI1QHfHrtyjlKNhYzG3IgHcfAZUURO16gFmWgzAZLkJSmCIxaIty/EmvG5N3ZePolBOa7lNEH/eSBMGAQteH+Twtiu0Y2xSwmmsxnfJyw== 2024-07-23T18:55:20Z KKBSTyiPKGkGl1AFqcPziKCEIDYGtnYUTQN4ukO7G40= CN=Trial LHDNM Sub CA V1, OU=Terms of use at http://www.posdigicert.com.my, O=LHDNM, C=MY 162880276254639189035871514749820882117 XML-SBDN12345 2024-07-23 00:40:00Z 13 MYR MYR 2024-07-01 2024-07-31 Monthly XML-SBINV12345 Reference Self-billed Invoice UUID 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 urn:oasis:names:specification:ubl:signature:Invoice urn:oasis:names:specification:ubl:dsig:enveloped:xades CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Self-Billed-Invoice-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-SBINV12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "11", "listVersionID": "1.1" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] } ], "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ], "DocumentType": [ { "\_": "CustomsImportForm" } ] }, { "ID": [ { "\_":



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Self-Billed-Invoice-Sample.xml

urn:oasis:names:specification:ubl:dsig:enveloped:xades urn:oasis:names:specification:ubl:signature:1 urn:oasis:names:specification:ubl:signature:Invoice not(//ancestor-or-self::ext:UBLExtensions) not(//ancestor-or-self::cac:Signature) 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 2024-07-23T18:42:14Z KKBSTyiPKGkGl1AFqcPziKCEIDYGtnYUTQN4ukO7G40= CN=Trial LHDNM Sub CA V1, OU=Terms of use at http://www.posdigicert.com.my, O=LHDNM, C=MY 162880276254639189035871514749820882117 XML-SBINV12345 2024-07-23 00:40:00Z 11 MYR MYR 2024-07-01 2024-07-31 Monthly 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 urn:oasis:names:specification:ubl:signature:Invoice urn:oasis:names:specification:ubl:dsig:enveloped:xades CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method is cash E12345678912 1.00 2024-07-23



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Self-Billed-Refund-Sample.json

{ "\_D": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2", "\_A": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2", "\_B": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2", "Invoice": [ { "ID": [ { "\_": "JSON-SBRN12345" } ], "IssueDate": [ { "\_": "2024-07-23" } ], "IssueTime": [ { "\_": "00:30:00Z" } ], "InvoiceTypeCode": [ { "\_": "14", "listVersionID": "1.1" } ], "DocumentCurrencyCode": [ { "\_": "MYR" } ], "TaxCurrencyCode": [ { "\_": "MYR" } ], "InvoicePeriod": [ { "StartDate": [ { "\_": "2024-01-01" } ], "EndDate": [ { "\_": "2024-07-31" } ], "Description": [ { "\_": "Monthly" } ] } ], "BillingReference": [ { "InvoiceDocumentReference": [ { "ID": [ { "\_": "JSON-SBINV12345" } ], "UUID": [ { "\_": "Reference Self-billed Invoice UUID" } ] } ] }, { "AdditionalDocumentReference": [ { "ID": [ { "\_": "E12345678912" } ] } ] }



---

## Source: https://sdk.myinvois.hasil.gov.my/files/sdksamples/1.1-Self-Billed-Refund-Sample.xml

urn:oasis:names:specification:ubl:dsig:enveloped:xades urn:oasis:names:specification:ubl:signature:1 urn:oasis:names:specification:ubl:signature:Invoice not(//ancestor-or-self::ext:UBLExtensions) not(//ancestor-or-self::cac:Signature) RfXFe2Sai6Z1ulzBtpBZhUymlleg1S5FaHfxB+UJuQc= vB3cA6nIudz3d6l9kmrAlsVeWmrG096p+nVg+HCdOPs= JXhPOtP3kDYOOPempTt03JNopZ6oN7+SRzKnnm81HJVwLhIM/zeKujx7EJ19fzFCtOjwxYvpvXo6jfjJ+ymDRE5vZBw7LjGq1X7s5PvDvyo/nLo8c7enhhCBm5D/XHFwpV/ZPToWercE8OUUdD2qemHRrObQEQ7vDtUcje3JK6oLDdWRba9kEk5ulrf3Nv/V8fFTpprCS64EIph1QhS6ngmZN2nBvfReAEZWUZ1LdxNdreyF5akY07DZ9GFy44BLFFmfFCSHDyXJO13XbYBSLZIy/cAT9N7t8sfhF7Z2PjrRbf7drp1f1jLBGesA6NfnmVC6xXeHYDKzxTyLnHTJRA== MIIFlDCCA3ygAwIBAgIQeomZorO+0AwmW2BRdWJMxTANBgkqhkiG9w0BAQsFADB1MQswCQYDVQQGEwJNWTEOMAwGA1UEChMFTEhETk0xNjA0BgNVBAsTLVRlcm1zIG9mIHVzZSBhdCBodHRwOi8vd3d3LnBvc2RpZ2ljZXJ0LmNvbS5teTEeMBwGA1UEAxMVVHJpYWwgTEhETk0gU3ViIENBIFYxMB4XDTI0MDYwNjAyNTIzNloXDTI0MDkwNjAyNTIzNlowgZwxCzAJBgNVBAYTAk1ZMQ4wDAYDVQQKEwVEdW1teTEVMBMGA1UEYRMMQzI5NzAyNjM1MDYwMRswGQYDVQQLExJUZXN0IFVuaXQgZUludm9pY2UxDjAMBgNVBAMTBUR1bW15MRIwEAYDVQQFEwlEMTIzNDU2NzgxJTAjBgkqhkiG9w0BCQEWFmFuYXMuYUBmZ3Zob2xkaW5ncy5jb20wggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQChvfOzAofnU60xFO7NcmF2WRi+dgor1D7ccISgRVfZC30Fdxnt1S6ZNf78Lbrz8TbWMicS8plh/pHy96OJvEBplsAgcZTd6WvaMUB2oInC86D3YShlthR6EzhwXgBmg/g9xprwlRqXMT2p4+K8zmyJZ9pIb8Y+tQNjm/uYNudtwGVm8A4hEhlRHbgfUXRzT19QZml6V2Ea0wQI8VyWWa8phCIkBD2w4F8jG4eP5/0XSQkTfBHHf+GV/YDJx5KiiYfmB1nGfwoPHix6Gey+wRjIq87on8Dm5+8ei8/bOhcuuSlpxgwphAP3rZrNbRN9LNVLSQ5md41asoBHfaDIVPVpAgMBAAGjgfcwgfQwHwYDVR0lBBgwFgYIKwYBBQUHAwQGCisGAQQBgjcKAwwwEQYDVR0OBAoECEDwms66hrpiMFMGA1UdIARMMEowSAYJKwYBBAGDikUBMDswOQYIKwYBBQUHAgEWLWh0dHBzOi8vd3d3LnBvc2RpZ2ljZXJ0LmNvbS5teS9yZXBvc2l0b3J5L2NwczATBgNVHSMEDDAKgAhNf9lrtsUI0DAOBgNVHQ8BAf8EBAMCBkAwRAYDVR0fBD0wOzA5oDegNYYzaHR0cDovL3RyaWFsY3JsLnBvc2RpZ2ljZXJ0LmNvbS5teS9UcmlhbExIRE5NVjEuY3JsMA0GCSqGSIb3DQEBCwUAA4ICAQBwptnIb1OA8NNVotgVIjOnpQtowew87Y0EBWAnVhOsMDlWXD/s+BL7vIEbX/BYa0TjakQ7qo4riSHyUkQ+X+pNsPEqolC4uFOp0pDsIdjsNB+WG15itnghkI99c6YZmbXcSFw9E160c7vG25gIL6zBPculHx5+laE59YkmDLdxx27e0TltUbFmuq3diYBOOf7NswFcDXCo+kXOwFfgmpbzYS0qfSoh3eZZtVHg0r6uga1UsMGb90+IRsk4st99EOVENvo0290lWhPBVK2G34+2TzbbYnVkoxnq6uDMw3cRpXX/oSfya+tyF51kT3iXvpmQ9OMF3wMlfKwCS7BZB2+iRja/1WHkAP7QW7/+0zRBcGQzY7AYsdZUllwYapsLEtbZBrTiH12X4XnZjny9rLfQLzJsFGT7Q+e02GiCsBrK7ZHNTindLRnJYAo4U2at5+SjqBiXSmz0DG+juOyFkwiWyD0xeheg4tMMO2pZ7clQzKflYnvFTEFnt+d+tvVwNjTboxfVxEv2qWF6qcMJeMvXwKTXuwVI2iUqmJSzJbUY+w3OeG7fvrhUfMJPM9XZBOp7CEI1QHfHrtyjlKNhYzG3IgHcfAZUURO16gFmWgzAZLkJSmCIxaIty/EmvG5N3ZePolBOa7lNEH/eSBMGAQteH+Twtiu0Y2xSwmmsxnfJyw== 2024-07-23T18:59:55Z KKBSTyiPKGkGl1AFqcPziKCEIDYGtnYUTQN4ukO7G40= CN=Trial LHDNM Sub CA V1, OU=Terms of use at http://www.posdigicert.com.my, O=LHDNM, C=MY 162880276254639189035871514749820882117 XML-SBRN12345 2024-07-23 00:40:00Z 14 MYR MYR 2024-07-01 2024-07-31 Monthly XML-SBINV12345 Reference Self-billed Invoice UUID 151891-1981 L1 CustomsImportForm FTA FreeTradeAgreement Sample Description L1 K2 L1 urn:oasis:names:specification:ubl:signature:Invoice urn:oasis:names:specification:ubl:dsig:enveloped:xades CPT-CCN-W-211111-KL-000002 46510 Supplier's TIN Supplier's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Supplier's Name +60123456789 supplier@email.com Buyer's TIN Buyer's BRN NA NA Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Buyer's Name +60123456780 buyer@email.com Recipient's TIN Recipient's BRN Kuala Lumpur 50480 14 Lot 66 Bangunan Merdeka Persiaran Jaya MYS Recipient's Name 1234 true Service charge 100 01 1234567890 Payment method



---

## Source: https://sdk.myinvois.hasil.gov.my/

Software Development Kit (SDK) for Lembaga Hasil Dalam Negeri Malaysia (LHDNM) MyInvois System Software Development Kit (SDK) for Lembaga Hasil Dalam Negeri Malaysia (LHDNM) MyInvois System ============================================================================================== MyInvois is the solution of the Lembaga Hasil Dalam Negeri Malaysia (LHDNM) used by taxpayers to submit their issued documents with the Tax Authority, get notified on events related to document issuance. This site contains documentation of the APIs exposed to taxpayer ERP systems that can be used to integrate with MyInvois System to automate the document processing. [Getting started...](/start/) [Lembaga Hasil Dalam Negeri Malaysia](https://www.hasil.gov.my/en/) This software development kit is provided by the Lembaga Hasil Dalam Negeri Malaysia. [Release Notes ------------- More information on the latest updates to MyInvois System and API Read



---

## Source: https://sdk.myinvois.hasil.gov.my/integration-practices/

Integration Practices * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Integration Practices ===================== This page explains about the Integration Practices that will help users to integrate with the API. [Postman](/postman/) Content ======= The solution supports multiple integration options, but it is important to integrate following the below guidance to make sure your integration is behaving correctly and you would be able to get the most benefits of the solution. Polling Approach ================ In this integration approach, the ERP system would submit documents using one of the submission APIs and then continue to check the status of these submitted documents using one of the submission APIs and the reference of the submission that was



---

## Source: https://sdk.myinvois.hasil.gov.my/mathematical-mappings/

Mathematical Mappings And Calculations * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Mathematical Mappings And Calculations ====================================== In order to perform mathematical mapping and calculation, follow these guidelines. | Element | Calculation Equation | | --- | --- | | Subtotal | (/ ubl:Invoice / cac:InvoiceLine / cac:Price / cbc:PriceAmount (Unit Price)) \* (/ ubl:Invoice / cac:InvoiceLine / cbc:InvoicedQuantity (Quantity)) | | Total Excluding Tax (Invoice Line Level) | (/ ubl:Invoice / cac:InvoiceLine / cac:ItemPriceExtension / cbc:Amount) (Subtotal) - SUM(/ ubl:Invoice / cac:InvoiceLine / cac:AllowanceCharge[ChargeIndicator=’false’] / cbc:Amount) (Discount Amount) + SUM(/ ubl:Invoice / cac:InvoiceLine / cac:AllowanceCharge[ChargeIndicator=’true’] / cbc:Amount) (Charge / Fee Amount) | | Total Excluding Tax (Invoice Level) | (/ ubl:Invoice /



---

## Source: https://sdk.myinvois.hasil.gov.my/postman

Postman * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Postman ======= Page describes about the Postman elements, creation and validation. [Digital Signature](/signature/) [Integration Practices](/integration-practices/) How to test APIs via Postman? ============================= For those that are using [Postman](https://www.postman.com/) to do quick tests and see how the APIs should be called both on identity service and actual document exchange, please use the Postman collection [e-Invoice SDK.postman\_collection.json](/files/EInvoicing SDK.postman_collection.json) (right-click to Save ) and use Postman as per the environment below (right-click to Save ). | Environment | Postman Env. File | | --- | --- | | PROD | [PROD Env.postman\_environment.json](/files/PROD Env.postman_environment.json) | | SANDBOX | [Sandbox Env.postman\_environment.json](/files/SANDBOX Env.postman_environment.json) | To install the environments file, follow



---

## Source: https://sdk.myinvois.hasil.gov.my/release-notes/

Release Notes * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Release Notes ============= This section contain new items related to SDK and technical aspects of the solution. SDK 1.0 Release --------------- • The SDK 1.0 was published on 6 April 2024. • Update was made on 19 April 2024. • Update was made on 10 May 2024. • Update was made on 24 May 2024. • Update was made on 21 Jun 2024. • Update was made on 28 Jun 2024. • Update was made on 10 August 2024. • Update was made on 10 October 2024. • Update was made on 28 December 2024. • Update was made on 14 January 2025.



---

## Source: https://sdk.myinvois.hasil.gov.my/sample/

Sample * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Sample ====== Page contain sample payload for each type of invoice [Digital Signature](/signature/) [Integration Practices](/integration-practices/) What are the available sample payload ===================================== The table below provides details about the available sample payload. | # | Filename | | --- | --- | | 1 | [Invoice 1.0 Sample XML](/files/sdksamples/1.0-Invoice-Sample.xml) | | 2 | [Invoice 1.0 Sample JSON](/files/sdksamples/1.0-Invoice-Sample.json) | | 3 | [Invoice 1.0 Foreign Currency Sample XML](/files/sdksamples/1.0-Invoice-ForeignCurrency-Sample.xml) | | 4 | [Invoice 1.0 Foreign Currency Sample JSON](/files/sdksamples/1.0-Invoice-ForeignCurrency-Sample.json) | | 5 | [Invoice 1.0 with Multi Line Item Sample XML](/files/sdksamples/1.0-Invoice-MultiLineItem-Sample.xml) | | 6 | [Invoice 1.0 with Multi Line Item Sample JSON](/files/sdksamples/1.0-Invoice-MultiLineItem-Sample.json) | | 7



---

## Source: https://sdk.myinvois.hasil.gov.my/sdk-(beta)-release/

Sdk (beta) Release * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Sdk (beta) Release ================== 09 Feb 2024 - Lembaga Hasil Dalam Negeri Malaysia Lembaga Hasil Dalam Negeri Malaysia has provisioned SDK (beta) Release to help taxpayers in preparing for the upcoming MyInvois System. Please note that this is a beta release which is subject to change as the solution evolves and more capabilities are added. Base URLs ========= In order for taxpayers to access the URLs for the various environments, please ensure that root certificate is trusted by the machine used to avoid any security-related issues accessing these URLs. See more in [FAQ](/faq/#how-to-set-up-environment-to-access-test-apis-and-test-portals). SDK Updates =========== TBD Document Version Updates ======================== TBD



---

## Source: https://sdk.myinvois.hasil.gov.my/sdk-1-0-release/

SDK 1.0 Release * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) SDK 1.0 Release =============== 01 Aug 2025 - Lembaga Hasil Dalam Negeri Malaysia Lembaga Hasil Dalam Negeri Malaysia has provisioned SDK 1.0 Release to help taxpayers in preparing for the upcoming MyInvois System. SDK Updates section below highlights key updates as part of this release. Base URLs ========= In order for taxpayers to access the URLs for the various environments, please ensure that root certificate is trusted by the machine used to avoid any security-related issues accessing these URLs. See more in [FAQ](/faq/#how-to-set-up-environment-to-access-test-apis-and-test-portals). SDK Updates =========== **9 August 2025** **Other Updates** • With reference to the release note issued on 1 August



---

## Source: https://sdk.myinvois.hasil.gov.my/signature-creation-json/

Signing a JSON document * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Signing a JSON document ======================= Introduction ------------ This page provides sample content on how to generate a signed version of a JSON document. This is assuming that the certificate has already been generated and is available as per the guidance provided here [Digital Signing Certificate Profile](https://sdk.myinvois.hasil.gov.my/signature/#digital-signing-certificate-profile) **Note: the code shown on this page is not production ready and hence not optimized for performance and is also missing errors and exceptions handling, please make sure you handle these points in your production ready code.** The following represents the steps required to be performed to generate the final signed JSON document including the



---

## Source: https://sdk.myinvois.hasil.gov.my/signature-creation/

Document Signature Creation * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Document Signature Creation =========================== Page describes the the algorithm of how signatures for documents submitted should be created. High-Level Process ================== The overall steps to take when preparing a single document for submission are: * **Step 1:** Create document XML or JSON (no signature elements yet) for a single document * **Step 2:** Apply transformations to the document * **Step 3:** Canonicalize the document and generate the document hash (digest) (property reference **DocDigest**) * **Step 4:** Sign the document digest (property reference **Sig**) * **Step 5:** Generate the certificate hash (Digest) (property reference **CertDigest**) * **Step 6:** Populate the signed properties section



---

## Source: https://sdk.myinvois.hasil.gov.my/signature/

Signature * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Signature ========= Page describes the signature elements, creation and validation. [FAQ](/faq/) [Postman](/postman/) Introduction ------------ This page provides guidance on the methods and approach that can be used to create digital signature for a document. This follows UBL 2.1 published standards as document here ([Universal Business Language Version 2.1](https://docs.oasis-open.org/ubl/UBL-2.1.html)) for XML and here ([UBL 2.1 JSON Alternative Representation Version 2.0](https://docs.oasis-open.org/ubl/UBL-2.1-JSON/v2.0/cnd01/UBL-2.1-JSON-v2.0-cnd01.html)) for JSON. The methods described in this page apply only to the documents that are submitted using the APIs described in this SDK as per the description here [Submit Documents](/einvoicingapi/02-submit-documents/) > The submitter of the documents will have to use a valid digital certificate that



---

## Source: https://sdk.myinvois.hasil.gov.my/standard-error-response/

Standard Error Response * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Standard Error Response ======================= Page describes the standard error data structure and standard error codes that APIs of e-Invoice are using. If there are specialized error code and messages for a specific API, these are defined in API definition page. Error Response Structure ======================== Error response is a single JSON object that has name value pair named `error`. This object can have the elements of type `Error` as defined in the table below. | Property | Type | Description | Value example | | --- | --- | --- | --- | | propertyName | String | The name of the target/subject



---

## Source: https://sdk.myinvois.hasil.gov.my/standard-header-parameters/

Standard Header Parameters * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Standard Header Parameters ========================== Page describes the standard header parameters that can be used by all APIs of the e-Invoice public API except those where explicitly stated otherwise. Request Header Parameters ========================= Any API Call ------------ These header parameters apply to all calls to all APIs if not explicitly stated otherwise. | Header parameter | Type | Description | Value example | | --- | --- | --- | --- | | Accept | String | Defines the content types that client is able to accept | application/json | | Accept-Language | String | May contain the preferred language for response. Supported



---

## Source: https://sdk.myinvois.hasil.gov.my/start/

Getting started... * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Getting started... ================== This page provides more information regarding the MyInvois System LHDNM MyInvois System ===================== To support the growth of the digital economy, the Government intends to implement e-Invoice in stages in an effort to enhance the efficiency of Malaysia’s tax administration management. This initiative is aligned with the Twelfth Malaysia Plan, which aims to strengthen the digital services infrastructure and modernise the tax administration system through digitalisation. The e-Invoice will enable near real-time validation and storage of transactions, catering to Business-to-Business (B2B), Business-to-Consumer (B2C) and Business-to-Government (B2G) transactions. Benefits of Adopting e-Invoice ------------------------------ The implementation of e-Invoice not only provides seamless



---

## Source: https://sdk.myinvois.hasil.gov.my/types/

Types * [Release Notes](/release-notes/) * [API](/api/) * [Types](/types/) * [Codes](/codes/) * [Validations](/document-validation-rules/) * [FAQ](/faq/) * [Contacts](/contacts/) Types ===== The section contains the definitions of the document structures that APIs can operate within the current version of the MyInvois System. The solution will support UBL 2.1 standards and would support both JSON and XML as described here [UBL-2.1](http://docs.oasis-open.org/ubl/UBL-2.1.html) and here [UBL-2.1-JSON-v2.0-cnd01.](https://docs.oasis-open.org/ubl/UBL-2.1-JSON/v2.0/cnd01/UBL-2.1-JSON-v2.0-cnd01.html) Please ensure to follow the right sequence of elements to match UBL 2.1 schema guidance. Invoice ------- Invoice is a commercial document issued by Supplier to itemise and record a transaction with Buyer. * [Invoice v1.0](/documents/invoice-v1-0/) v1.0 of the Invoice document type structure is maintained as v1.1, the only difference is that signature validation is disabled on this version. This

