Cancel Document

* [Release Notes](/release-notes/)
* [API](/api/)
* [Types](/types/)
* [Codes](/codes/)
* [Validations](/document-validation-rules/)
* [FAQ](/faq/)
* [Contacts](/contacts/)

Cancel Document
===============

This API allows issuer to cancel previously issued document, either self-induced cancellation or by accepting a rejection request made by the buyer.

[Submit Documents](/einvoicingapi/02-submit-documents/)
[Reject Document](/einvoicingapi/04-reject-document/)

Overview
--------

Document cancellation is a way to correct submission errors that were noticed right away. Ideally, cancellation is done even before the document is fully validated and recipient is notified. Therefore, cancellation can be done only within limited time period from the validation of the document. This time limit is specific to document type and is returned by calling [Get Document Type API](/api/04-get-document-type/) and checking workflow parameters.

Cancellation is permitted within the 72-hour window from the date and time the document was marked as valid. If cancellation time has passed, taxpayers can revert / adjust the previously issued incorrect invoice through submission of a credit note/debit note/refund note (as the case may be).

**Note!** When you are logged in as intermediary, permissions that are granted by the taxpayer will be applied on your profile and this will control the functionalities that you'll be able to executed on behalf of the taxpayer you are representing.

Signature
---------

This is REST based API that receives the document ID through the URL parameter and state to be changed in request body.

Signature:
`PUT /api/v1.0/documents/state/{UUID}/state`

Rate Limit
----------

To optimize the use of our APIs, a rate limit of 12 Requests Per Minute (RPM) / Client ID is recommended.

Inputs
------

This API accepts [standard e-Invoice API header parameters](/standard-header-parameters/) for authenticated call.

| URL parameter | Type | Description | Value example | Requirement |
| --- | --- | --- | --- | --- |
| uuid | String | Unique ID of existing document. | F9D425P6DS7D8IU | Mandatory |

| Body parameter | Type | Description | Value example | Requirement |
| --- | --- | --- | --- | --- |
| status | String | Desired status for the document. Must be `cancelled` to cancel previously issued document. | cancelled | Mandatory |
| reason | String | Reason for cancelling the document.  (The length of the reason would be limited to 300 chars) | Customer cancelled the order. Examples of reasons: `Wrong buyer details` or `Wrong invoice details` or any other reasons as the supplier deems appropriate | Mandatory |

Outputs
-------

| Parameter | Type | Description | Value example |
| --- | --- | --- | --- |
| uuid | String | Unique ID of the document | F9D425P6DS7D8IU |
| status | String | Status if document has been cancelled | Cancelled |
| error | [Error](/standard-error-response/#error-response-structure) | Error if cancellion of document failed. |  |

### Successful Response

On a successful submission, this API returns `200` status code.

### Error Response

Error situations are reported back by this API through the [standard error response](/standard-error-response/).

Additional specialised error messages can be returned as a result of validation of state of the document and caller:

| HTTP Status Code | Error Code | Description |
| --- | --- | --- |
| 400 | OperationPeriodOver | Returned when user is trying to cancel document when the time limit of cancellation has already run out. |
| 400 | IncorrectState | Returned when caller is trying to cancel the document that might already be rejected or invalid. State transition in this case is not allowed. |
| 400 | ActiveReferencingDocuments | Returned when caller is trying to cancel the document that has been referenced by other documents, e.g., credit note referencing invoice. The required action is to first cancel the referencing document and followed by this one. |
| 403 | Forbidden | Returned when valid taxpayer system is trying to perform operation on a document not issued by them. |

Additional considerations
-------------------------

In case of self-billed invoices, the buyer actually cancels the document, not the supplier.

Notes
-----

**Important !**

• Please ensure the UUID is correct before attempting to cancel a submission to avoid unnecessary API calls.

• Always review the integration recommended practices at [sdk.myinvois.hasil.gov.my/integration-practices](https://sdk.myinvois.hasil.gov.my/integration-practices) to ensure your ERP integration is in accordance with these guidelines and follows healthy integration patterns.

[Back to homepage](/)