<a name="module_sv-api"></a>
## sv-api
Exposes operations supported by StudentVerification RESTful API.


* [sv-api](#module_sv-api)
  * [~isirs](#module_sv-api..isirs)
    * [new isirs()](#new_module_sv-api..isirs_new)
    * [.upload(rootUrl, authorization, awardYear, content)](#module_sv-api..isirs.upload) ⇒ <code>function</code>
    * [.getCorrections(rootUrl, authorization, startDate, endDate, targetPath)](#module_sv-api..isirs.getCorrections) ⇒ <code>function</code>
  * [~documents](#module_sv-api..documents)
    * [new documents()](#new_module_sv-api..documents_new)
    * [.getMetadata(rootUrl, authorization, documentId)](#module_sv-api..documents.getMetadata) ⇒ <code>function</code>
    * [.getFiles(rootUrl, authorization, documentId, targetPath)](#module_sv-api..documents.getFiles) ⇒ <code>function</code>
    * [.get()](#module_sv-api..documents.get) ⇒ <code>function</code>
  * [~requirements](#module_sv-api..requirements)
    * [new requirements()](#new_module_sv-api..requirements_new)

<a name="module_sv-api..isirs"></a>
### sv-api~isirs
**Kind**: inner class of <code>[sv-api](#module_sv-api)</code>  

* [~isirs](#module_sv-api..isirs)
  * [new isirs()](#new_module_sv-api..isirs_new)
  * [.upload(rootUrl, authorization, awardYear, content)](#module_sv-api..isirs.upload) ⇒ <code>function</code>
  * [.getCorrections(rootUrl, authorization, startDate, endDate, targetPath)](#module_sv-api..isirs.getCorrections) ⇒ <code>function</code>

<a name="new_module_sv-api..isirs_new"></a>
#### new isirs()
Represents functions associated with ISIR files

<a name="module_sv-api..isirs.upload"></a>
#### isirs.upload(rootUrl, authorization, awardYear, content) ⇒ <code>function</code>
upload a file as application/octet-stream content

**Kind**: static method of <code>[isirs](#module_sv-api..isirs)</code>  
**Returns**: <code>function</code> - A promise.

| Param | Type | Description |
| --- | --- | --- |
| rootUrl | <code>string</code> | url of awardletter API |
| authorization | <code>string</code> | header value |
| awardYear | <code>string</code> | Award/aid year in [YYYY]-[YYYY] format; ex. 2015-2016 |
| content | <code>object</code> | JSON content to be uploaded |

<a name="module_sv-api..isirs.getCorrections"></a>
#### isirs.getCorrections(rootUrl, authorization, startDate, endDate, targetPath) ⇒ <code>function</code>
Get batched ISIR corrections for a given start date and end date

**Kind**: static method of <code>[isirs](#module_sv-api..isirs)</code>  
**Returns**: <code>function</code> - A promise.

| Param | Type | Description |
| --- | --- | --- |
| rootUrl | <code>string</code> | url of awardletter API |
| authorization | <code>string</code> | header value |
| startDate | <code>string</code> | A start date in MM-DD-YYYY format |
| endDate | <code>string</code> | An end date in MM-DD-YYYY format |
| targetPath | <code>string</code> | An optional target path in which files will be written |

<a name="module_sv-api..documents"></a>
### sv-api~documents
**Kind**: inner class of <code>[sv-api](#module_sv-api)</code>  

* [~documents](#module_sv-api..documents)
  * [new documents()](#new_module_sv-api..documents_new)
  * [.getMetadata(rootUrl, authorization, documentId)](#module_sv-api..documents.getMetadata) ⇒ <code>function</code>
  * [.getFiles(rootUrl, authorization, documentId, targetPath)](#module_sv-api..documents.getFiles) ⇒ <code>function</code>
  * [.get()](#module_sv-api..documents.get) ⇒ <code>function</code>

<a name="new_module_sv-api..documents_new"></a>
#### new documents()
Represents functions associated with student documents

<a name="module_sv-api..documents.getMetadata"></a>
#### documents.getMetadata(rootUrl, authorization, documentId) ⇒ <code>function</code>
Get student document metadata.

**Kind**: static method of <code>[documents](#module_sv-api..documents)</code>  
**Returns**: <code>function</code> - A promise.

| Param | Type | Description |
| --- | --- | --- |
| rootUrl | <code>string</code> | url of awardletter API |
| authorization | <code>string</code> | header value |
| documentId | <code>string</code> | The unique Id of the student document |

<a name="module_sv-api..documents.getFiles"></a>
#### documents.getFiles(rootUrl, authorization, documentId, targetPath) ⇒ <code>function</code>
[getFiles description]

**Kind**: static method of <code>[documents](#module_sv-api..documents)</code>  
**Returns**: <code>function</code> - A promise.

| Param | Type |
| --- | --- |
| rootUrl | <code>string</code> | 
| authorization | <code>string</code> | 
| documentId | <code>string</code> | 
| targetPath | <code>string</code> | 

<a name="module_sv-api..documents.get"></a>
#### documents.get() ⇒ <code>function</code>
Get student document metadata and associated file(s).

**Kind**: static method of <code>[documents](#module_sv-api..documents)</code>  
**Returns**: <code>function</code> - A promise.
<a name="module_sv-api..requirements"></a>
### sv-api~requirements
**Kind**: inner class of <code>[sv-api](#module_sv-api)</code>  
<a name="new_module_sv-api..requirements_new"></a>
#### new requirements()
Represents functions associated with student requirements/tasks
