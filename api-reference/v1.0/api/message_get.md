# <a name="get-message"></a><span data-ttu-id="1a6af-101">Nachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="1a6af-101">Get message</span></span>

<span data-ttu-id="1a6af-102">Mit dieser Methode können Sie die Eigenschaften und Beziehungen eines [message](../resources/message.md)-Objekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="1a6af-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="1a6af-103">Zurzeit gibt dieser Vorgang Nachrichtentext ausschließlich im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="1a6af-103">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="1a6af-104">Es gibt zwei Szenarien, in denen eine App eine Nachricht im E-Mail-Ordner eines anderen Benutzers erhalten kann:</span><span class="sxs-lookup"><span data-stu-id="1a6af-104">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="1a6af-105">Wenn die App über Anwendungsberechtigungen verfügt oder</span><span class="sxs-lookup"><span data-stu-id="1a6af-105">If the app has application permissions, or,</span></span>
* <span data-ttu-id="1a6af-106">Wenn die App über die entsprechenden delegierten [Berechtigungen](#permissions)  von einem Benutzer verfügt und ein anderer Benutzer einen E-Mail-Ordner für diesen Benutzer freigegeben hat oder delegierten Zugriff auf diesen Benutzer gewährt hat.</span><span class="sxs-lookup"><span data-stu-id="1a6af-106">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="1a6af-107">|||UNTRANSLATED_CONTENT_START|||See [details and an example](../../../concepts/outlook-share-messages-folders.md).|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="1a6af-107">See [details and an example](../../../concepts/outlook-share-messages-folders.md).</span></span>

<span data-ttu-id="1a6af-108">|||UNTRANSLATED_CONTENT_START|||Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="1a6af-108">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="1a6af-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1a6af-109">Permissions</span></span>
<span data-ttu-id="1a6af-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1a6af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1a6af-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1a6af-112">Permission type</span></span>      | <span data-ttu-id="1a6af-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1a6af-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a6af-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1a6af-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1a6af-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1a6af-115">Mail.Read</span></span>    |
|<span data-ttu-id="1a6af-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1a6af-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a6af-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1a6af-117">Mail.Read</span></span>    |
|<span data-ttu-id="1a6af-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1a6af-118">Application</span></span> | <span data-ttu-id="1a6af-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1a6af-119">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a6af-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a6af-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1a6af-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1a6af-121">Optional query parameters</span></span>
<span data-ttu-id="1a6af-122">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1a6af-122">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1a6af-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1a6af-123">Request headers</span></span>
| <span data-ttu-id="1a6af-124">Name</span><span class="sxs-lookup"><span data-stu-id="1a6af-124">Name</span></span>       | <span data-ttu-id="1a6af-125">Typ</span><span class="sxs-lookup"><span data-stu-id="1a6af-125">Type</span></span> | <span data-ttu-id="1a6af-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a6af-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1a6af-127">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1a6af-127">Authorization</span></span>  | <span data-ttu-id="1a6af-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a6af-128">string</span></span>  | <span data-ttu-id="1a6af-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1a6af-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1a6af-131">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="1a6af-131">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="1a6af-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a6af-132">string</span></span> | <span data-ttu-id="1a6af-133">Das Format, in der die **body**- und **uniqueBody**-Eigenschaften zurückgegeben werden sollen.</span><span class="sxs-lookup"><span data-stu-id="1a6af-133">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="1a6af-134">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="1a6af-134">Values can be "text" or "html".</span></span> <span data-ttu-id="1a6af-135">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="1a6af-135">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="1a6af-136">Wenn die Kopfzeile nicht angegeben ist, werden die **body**- und **uniqueBody**-Eigenschaften im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a6af-136">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="1a6af-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="1a6af-137">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a6af-138">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1a6af-138">Request body</span></span>
<span data-ttu-id="1a6af-139">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1a6af-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a6af-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a6af-140">Response</span></span>

<span data-ttu-id="1a6af-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a6af-141">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1a6af-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1a6af-142">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="1a6af-143">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="1a6af-143">Request 1</span></span>
<span data-ttu-id="1a6af-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1a6af-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
##### <a name="response-1"></a><span data-ttu-id="1a6af-145">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="1a6af-145">Response 1</span></span>
<span data-ttu-id="1a6af-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a6af-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuZ\"",
    "id":"AAMkADhMGAAA=",
    "createdDateTime":"2018-09-09T03:15:05Z",
    "lastModifiedDateTime":"2018-09-09T03:15:08Z",
    "changeKey":"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuZ",
    "categories":[

    ],
    "receivedDateTime":"2018-09-09T03:15:08Z",
    "sentDateTime":"2018-09-09T03:15:06Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR6E1BE060@MWHPR1120.namprd22.prod.outlook.com>",
    "subject":"9/9/2018: concert",
    "bodyPreview":"The group represents Nevada.",
    "importance":"normal",
    "parentFolderId":"AAMkADcbAAAAAAEJAAA=",
    "conversationId":"AAQkADOUpag6yWs=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADMGAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThe group represents Nevada.\r\n</body>\r\n</html>\r\n"
    },
    "sender":{
        "emailAddress":{
            "name":"Adele Vance",
            "address":"adelev@contoso.OnMicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Adele Vance",
            "address":"adelev@contoso.OnMicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="1a6af-149">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="1a6af-149">Request 2</span></span>
<span data-ttu-id="1a6af-150">Beim nächsten Beispiel werden die Kopfzeilen einer Internet-Nachricht mithilfe eines `$select` Abfrageparameters ermittelt.</span><span class="sxs-lookup"><span data-stu-id="1a6af-150">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
##### <a name="response-2"></a><span data-ttu-id="1a6af-151">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="1a6af-151">Response 2</span></span>
<span data-ttu-id="1a6af-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1a6af-152">Here is an example of the response.</span></span> <span data-ttu-id="1a6af-153">Hinweis: Die Gruppe der Nachrichten-Kopfzeilen im Antwortobjekt wurde aus Platzgründen gekürzt.</span><span class="sxs-lookup"><span data-stu-id="1a6af-153">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="1a6af-154">Alle Header werden von einem aktuellen Anruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a6af-154">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages(internetMessageHeaders)/$entity",
    "@odata.etag":"W/\"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB\"",
    "id":"AAMkADhAAAW-VPeAAA=",
    "internetMessageHeaders":[
        {
            "name":"MIME-Version",
            "value":"1.0"
        },
        {
            "name":"Content-Type",
            "value":"multipart/report"
        },
        {
            "name":"x-custom-header-group-name",
            "value":"Washington"
        },
        {
            "name":"x-custom-header-group-id",
            "value":"WA001"
        }
    ]
}
```


## <a name="see-also"></a><span data-ttu-id="1a6af-155">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="1a6af-155">See also</span></span>

- [<span data-ttu-id="1a6af-156">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="1a6af-156">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="1a6af-157">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="1a6af-157">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
