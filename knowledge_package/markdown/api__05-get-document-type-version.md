Get Document Type Version

* [Release Notes](/release-notes/)
* [API](/api/)
* [Types](/types/)
* [Codes](/codes/)
* [Validations](/document-validation-rules/)
* [FAQ](/faq/)
* [Contacts](/contacts/)

Get Document Type Version
=========================

This API allows taxpayer's ERP system to retrieve the details of document type version that contains structure definitions of the documents.

[Get Document Type](/api/04-get-document-type/)
[Get Notifications](/api/06-get-notifications/)

Overview
--------

This API allows taxpayer ERP system to retrieve the details of document type version that contains structure definitions of the documents that are expected to be submitted as part of [document submission](/einvoicingapi/02-submit-documents/).

Document type versions are used to allow document type data fields to be evolved over time without introducing a new document type. For example, if the document type version 1.0 include optional field(s), such field(s) could at a later time be made mandatory in document type version 2.0

Note that it is possible for one document type to have multiple valid document type versions to ease transition. In other words, taxpayers would still be able to submit old versions for validation despite the new / updated version has been deployed. It is however suggested for the taxpayers to migrate to the latest document type version as soon as possible.

Signature
---------

This is REST based API that takes unique ID of the document type and ID of the document type as URL parameter and returns full document type version object.

Signature:
`GET /api/v1.0/documenttypes/{id}/versions/{vid}`

Inputs
------

This API accepts [standard e-Invoice API header parameters](/standard-header-parameters/) for authenticated call.

| URL parameter | Type | Description | Value example | Requirement |
| --- | --- | --- | --- | --- |
| id | Number | Unique ID of existing document type | 45 | Mandatory |
| vid | Number | Unique ID of existing document type version that is published or deactivated | 41235 | Mandatory |

Outputs
-------

### Successful Response

This API returns HTTP status code `200`.

The resulting structure is a single object of type `DocumentTypeVersion`.

Document Type Version contains:

| Output parameter | Type | Description | Value example |
| --- | --- | --- | --- |
| [invoiceTypeCode](/codes/e-invoice-types/) | Number | The document type code from the possible values: `01`,`02`,`03`,`04`,`11`,`12`,`13`,`14` | 04 |
| name | String | Name of the document type version within the document type that can be used in document submission to identify document type version being submitted | 1.0 |
| description | String | Description of the document type version | Credit note version 1.0 |
| versionNumber | Decimal | Unique version number of the document type version that can be sorted to find the latest version | 1.0 |
| status | String | Status of the document type version - “published”, “deactivated” | published |
| activeFrom | Date | Date when the activity of the document type version started | 2015-02-13T13:15:00Z |
| activeTo | Date | Optional: date when the activity of the document type version sends/when it was deactivated | 2027-03-01T00:00:00Z |

### Error Response

Error situations are reported back by this API through the [standard error response](/standard-error-response/).

No custom error codes are provided by this API.

Additional considerations
-------------------------

To get the ID used to call this API, taxpayer system needs to first call API returning list of the [document types and their versions](/api/03-get-document-types/).

[Back to homepage](/)