Get All Document Types

* [Release Notes](/release-notes/)
* [API](/api/)
* [Types](/types/)
* [Codes](/codes/)
* [Validations](/document-validation-rules/)
* [FAQ](/faq/)
* [Contacts](/contacts/)

Get All Document Types
======================

This API allows taxpayer's systems to retrieve list of document types published by the MyInvois System.

[Login as Intermediary System](/api/08-login-as-intermediary-system/)
[Get Document Type](/api/04-get-document-type/)

Overview
--------

The main function of the MyInvois System is to enable submission of the issued documents to tax authority. There are multiple types of documents supported by the solution and this API allows taxpayer ERP systems to retrieve their definitions through API call.

Signature
---------

This is REST based API that does not take additional URL parameters, yet it returns the list of active and deactivated document types that were once active.

Signature:
`GET /api/v1.0/documenttypes`

Inputs
------

This API accepts [standard e-Invoice API header parameters](/standard-header-parameters/) for authenticated call.

No additional URL or request body parameters are provided to this API.

Outputs
-------

### Successful Response

This API returns HTTP status code `200`.

The resulting structure is part of a single object `result` that includes list of `DocumentType` elements.

Output list of Document Types contains:

| Output parameter | Type | Description | Value example |
| --- | --- | --- | --- |
| id | Number | Unique identifier of the document type | 45 |
| [invoiceTypeCode](/codes/e-invoice-types/) | Number | The document type code from the possible values: `1`,`2`,`3`,`4`,`11`,`12`,`13`,`14` | 04 |
| description | String | Description of the document type | Invoice |
| activeFrom | Date | Date when the activity of the document type started | 2015-02-13T13:15:00Z |
| activeTo | Date | Optional: date when the activity of the document type ends | 2027-03-01T00:00:00Z |
| documentTypeVersions | Array of document type version summary objects | 1 or more array values |  |

Array of document type version summary objects contains:

| Output parameter | Type | Description | Value example |
| --- | --- | --- | --- |
| id | Number | Unique identifier of the document type version | 454 |
| name | String | Unique name of the document type version | 1.0 |
| description | String | Description of the document type version | Invoice version 1.1 |
| activeFrom | Date | Date when the activity of the document type version started | 2015-02-13T13:15:00Z |
| activeTo | Date | Optional: date when the activity of the document type version ends | 2027-03-01T00:00:00Z |
| versionNumber | Decimal | Unique version number of the document type version | 1.1 |
| status | String | Status of the document type version - `draft`, `published`, `deactivated` | published |

### Error Response

Error situations are reported back by this API through the [standard error response](/standard-error-response/).

No custom error codes are provided by this API.

Additional considerations
-------------------------

When document type list is returned to caller, they can query more detailed information about [document type](/api/04-get-document-type/) or [document type version](/api/05-get-document-type-version/) using returned internal identifiers.

[Back to homepage](/)