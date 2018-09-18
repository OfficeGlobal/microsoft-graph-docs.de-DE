# <a name="get-message"></a><span data-ttu-id="e8669-101">Nachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="e8669-101">Get message</span></span>

<span data-ttu-id="e8669-102">Mit dieser Methode können Sie die Eigenschaften und Beziehungen eines [message](../resources/message.md)-Objekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="e8669-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="e8669-103">Da die **message**-Ressource [Erweiterungen](../../../concepts/extensibility_overview.md) unterstützt, können Sie über den `GET`-Vorgang auch benutzerdefinierte Eigenschaften und Erweiterungsdaten aus **message**-Instanzen abrufen.</span><span class="sxs-lookup"><span data-stu-id="e8669-103">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>

<span data-ttu-id="e8669-104">Zurzeit gibt dieser Vorgang Nachrichtentext ausschließlich im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="e8669-104">Currently, this operation returns message bodies in only HTML format.</span></span>


### <a name="get-messages-in-another-users-message-folder"></a><span data-ttu-id="e8669-105">Anzeigen von Nachrichten im Nachrichtenordner eines anderen Benutzers</span><span class="sxs-lookup"><span data-stu-id="e8669-105">Get messages in another user's message folder</span></span>

<span data-ttu-id="e8669-106">Wenn Sie über Anwendungsberechtigungen oder die entsprechenden delegierten [Berechtigungen](#permissions) eines Benutzers verfügen, können Sie Nachrichten aus dem Nachrichtenordner eines anderen Benutzers anzeigen.</span><span class="sxs-lookup"><span data-stu-id="e8669-106">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get messages from another user's message folder.</span></span> <span data-ttu-id="e8669-107">Dieser Abschnitt enthält Szenarien zu delegierten Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="e8669-107">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="e8669-108">Beispiel: Ihre App besitzt delegierte Berechtigungen des Benutzers John.</span><span class="sxs-lookup"><span data-stu-id="e8669-108">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="e8669-109">Der Benutzer Garth hat einen Nachrichtenordner für John freigegeben.</span><span class="sxs-lookup"><span data-stu-id="e8669-109">Suppose another user, Garth, has shared a message folder with John.</span></span> <span data-ttu-id="e8669-110">Sie können eine Nachricht in diesem freigegebenen Ordner aufrufen, indem Sie Garths Benutzer-ID (oder den Benutzerprinzipalnamen) in der unten gezeigten Beispielabfrage angeben.</span><span class="sxs-lookup"><span data-stu-id="e8669-110">You can get a message in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/messages/{id}
```

<span data-ttu-id="e8669-111">Diese Funktion gilt für alle unterstützten GET-Nachrichtenvorgänge für einen einzelnen Benutzer (siehe Abschnitt [HTTP-Anforderung](#http-request) unten).</span><span class="sxs-lookup"><span data-stu-id="e8669-111">This capability applies to all the supported GET messages operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="e8669-112">Sie gilt auch, wenn Garth sein gesamtes Postfach an John delegiert hat.</span><span class="sxs-lookup"><span data-stu-id="e8669-112">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="e8669-113">Wenn Garth weder seinen Nachrichtenordner für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8669-113">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="e8669-114">In solchen Fällen funktioniert die Angabe einer Benutzer-ID oder eines Benutzerprinzipalnamens nur, um Nachrichten aus dem Nachrichtenordner eines angemeldeten Benutzers anzuzeigen, und die Abfrage entspricht der Verwendung der Verknüpfung the /me:</span><span class="sxs-lookup"><span data-stu-id="e8669-114">In such cases, specifying a user ID or user principal name only works for getting a message in the signed-in user’s own message folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
```

<span data-ttu-id="e8669-115">Diese Funktion ist nur in GET-Vorgängen verfügbar für:</span><span class="sxs-lookup"><span data-stu-id="e8669-115">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="e8669-116">Freigegebene Kontaktordner, Kalender und Nachrichtenordner</span><span class="sxs-lookup"><span data-stu-id="e8669-116">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="e8669-117">Kontakte, Ereignisse und Nachrichten in freigegebenen Ordnern</span><span class="sxs-lookup"><span data-stu-id="e8669-117">Contacts, events, and messages in shared folders</span></span>
- <span data-ttu-id="e8669-118">Die oben aufgeführten Ressourcen in delegierten Postfächern</span><span class="sxs-lookup"><span data-stu-id="e8669-118">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="e8669-119">Diese Funktion steht in anderen Vorgängen für Kontakte, Ereignisse, Nachrichten und deren Ordner nicht zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="e8669-119">This capability is not available in other operations for contacts, events, messages, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="e8669-120">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e8669-120">Permissions</span></span>
<span data-ttu-id="e8669-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e8669-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e8669-123">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e8669-123">Permission type</span></span>      | <span data-ttu-id="e8669-124">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e8669-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8669-125">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e8669-125">Delegated (work or school account)</span></span> | <span data-ttu-id="e8669-126">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e8669-126">Mail.Read</span></span>    |
|<span data-ttu-id="e8669-127">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e8669-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8669-128">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e8669-128">Mail.Read</span></span>    |
|<span data-ttu-id="e8669-129">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e8669-129">Application</span></span> | <span data-ttu-id="e8669-130">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e8669-130">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8669-131">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8669-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e8669-132">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e8669-132">Optional query parameters</span></span>
<span data-ttu-id="e8669-133">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e8669-133">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e8669-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e8669-134">Request headers</span></span>
| <span data-ttu-id="e8669-135">Name</span><span class="sxs-lookup"><span data-stu-id="e8669-135">Name</span></span>       | <span data-ttu-id="e8669-136">Typ</span><span class="sxs-lookup"><span data-stu-id="e8669-136">Type</span></span> | <span data-ttu-id="e8669-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8669-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e8669-138">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e8669-138">Authorization</span></span>  | <span data-ttu-id="e8669-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8669-139">string</span></span>  | <span data-ttu-id="e8669-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e8669-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e8669-142">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="e8669-142">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="e8669-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8669-143">string</span></span> | <span data-ttu-id="e8669-144">Das Format, in der die **body**- und **uniqueBody**-Eigenschaften zurückgegeben werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e8669-144">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="e8669-145">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="e8669-145">Values can be "text" or "html".</span></span> <span data-ttu-id="e8669-146">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="e8669-146">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="e8669-147">Wenn die Kopfzeile nicht angegeben ist, werden die **body**- und **uniqueBody**-Eigenschaften im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8669-147">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="e8669-148">Optional.</span><span class="sxs-lookup"><span data-stu-id="e8669-148">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8669-149">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e8669-149">Request body</span></span>
<span data-ttu-id="e8669-150">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e8669-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8669-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8669-151">Response</span></span>

<span data-ttu-id="e8669-152">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8669-152">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e8669-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e8669-153">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="e8669-154">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="e8669-154">Request 1</span></span>
<span data-ttu-id="e8669-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e8669-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
##### <a name="response-1"></a><span data-ttu-id="e8669-156">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="e8669-156">Response 1</span></span>
<span data-ttu-id="e8669-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8669-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="e8669-160">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="e8669-160">Request 2</span></span>
<span data-ttu-id="e8669-161">Beim nächsten Beispiel werden die Kopfzeilen einer Internet-Nachricht mithilfe eines `$select` Abfrageparameters ermittelt.</span><span class="sxs-lookup"><span data-stu-id="e8669-161">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
##### <a name="response-2"></a><span data-ttu-id="e8669-162">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="e8669-162">Response 2</span></span>
<span data-ttu-id="e8669-163">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e8669-163">Here is an example of the response.</span></span> <span data-ttu-id="e8669-164">Hinweis: Die Gruppe der Nachrichten-Kopfzeilen im Antwortobjekt wurde aus Platzgründen gekürzt.</span><span class="sxs-lookup"><span data-stu-id="e8669-164">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="e8669-165">Von einem tatsächlichen Aufruf werden alle Kopfzeilen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8669-165">All of the properties will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="e8669-166">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="e8669-166">See also</span></span>

- [<span data-ttu-id="e8669-167">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="e8669-167">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="e8669-168">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="e8669-168">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
