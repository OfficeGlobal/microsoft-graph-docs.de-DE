# <a name="get-message"></a><span data-ttu-id="9f713-101">Nachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="9f713-101">Get message</span></span>

<span data-ttu-id="9f713-102">Mit dieser Methode können Sie die Eigenschaften und Beziehungen eines [message](../resources/message.md)-Objekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="9f713-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="9f713-103">Da die **message**-Ressource [Erweiterungen](../../../concepts/extensibility_overview.md) unterstützt, können Sie über den `GET`-Vorgang auch benutzerdefinierte Eigenschaften und Erweiterungsdaten aus **message**-Instanzen abrufen.</span><span class="sxs-lookup"><span data-stu-id="9f713-103">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>

<span data-ttu-id="9f713-104">Zurzeit gibt dieser Vorgang Nachrichtentext ausschließlich im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="9f713-104">Currently, this operation returns message bodies in only HTML format.</span></span>


### <a name="get-messages-in-another-users-message-folder"></a><span data-ttu-id="9f713-105">Anzeigen von Nachrichten im Nachrichtenordner eines anderen Benutzers</span><span class="sxs-lookup"><span data-stu-id="9f713-105">Get messages in another user's message folder</span></span>

<span data-ttu-id="9f713-106">Wenn Sie über Anwendungsberechtigungen oder die entsprechenden delegierten [Berechtigungen](#permissions) eines Benutzers verfügen, können Sie Nachrichten aus dem Nachrichtenordner eines anderen Benutzers anzeigen.</span><span class="sxs-lookup"><span data-stu-id="9f713-106">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get contacts from another user's contact folder.</span></span> <span data-ttu-id="9f713-107">Dieser Abschnitt enthält Szenarien zu delegierten Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="9f713-107">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="9f713-108">Beispiel: Ihre App besitzt delegierte Berechtigungen des Benutzers John.</span><span class="sxs-lookup"><span data-stu-id="9f713-108">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="9f713-109">Der Benutzer Garth hat einen Nachrichtenordner für John freigegeben.</span><span class="sxs-lookup"><span data-stu-id="9f713-109">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="9f713-110">Sie können eine Nachricht in diesem freigegebenen Ordner aufrufen, indem Sie Garths Benutzer-ID (oder den Benutzerprinzipalnamen) in der unten gezeigten Beispielabfrage angeben.</span><span class="sxs-lookup"><span data-stu-id="9f713-110">You can get a contact in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/messages/{id}
```

<span data-ttu-id="9f713-111">Diese Funktion gilt für alle unterstützten GET-Nachrichtenvorgänge für einen einzelnen Benutzer (siehe Abschnitt [HTTP-Anforderung](#http-request) unten).</span><span class="sxs-lookup"><span data-stu-id="9f713-111">This capability applies to all the supported GET contacts operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="9f713-112">Sie gilt auch, wenn Garth sein gesamtes Postfach an John delegiert hat.</span><span class="sxs-lookup"><span data-stu-id="9f713-112">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="9f713-113">Wenn Garth weder seinen Nachrichtenordner für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f713-113">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="9f713-114">In solchen Fällen funktioniert die Angabe einer Benutzer-ID oder eines Benutzerprinzipalnamens nur, um Nachrichten aus dem Nachrichtenordner eines angemeldeten Benutzers anzuzeigen, und die Abfrage entspricht der Verwendung der Verknüpfung the /me:</span><span class="sxs-lookup"><span data-stu-id="9f713-114">In such cases, specifying a user ID or user principal name only works for getting a contact in the signed-in user’s own contact folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
```

<span data-ttu-id="9f713-115">Diese Funktion ist nur in GET-Vorgängen verfügbar für:</span><span class="sxs-lookup"><span data-stu-id="9f713-115">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="9f713-116">Freigegebene Kontaktordner, Kalender und Nachrichtenordner</span><span class="sxs-lookup"><span data-stu-id="9f713-116">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="9f713-117">Kontakte, Ereignisse und Nachrichten in freigegebenen Ordnern</span><span class="sxs-lookup"><span data-stu-id="9f713-117">Contacts and events in shared folders</span></span>
- <span data-ttu-id="9f713-118">Die oben aufgeführten Ressourcen in delegierten Postfächern</span><span class="sxs-lookup"><span data-stu-id="9f713-118">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="9f713-119">Diese Funktion steht in anderen Vorgängen für Kontakte, Ereignisse, Nachrichten und deren Ordner nicht zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="9f713-119">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="9f713-120">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9f713-120">Permissions</span></span>
<span data-ttu-id="9f713-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9f713-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9f713-123">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f713-123">Permission type</span></span>      | <span data-ttu-id="9f713-124">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f713-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f713-125">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f713-125">Delegated (work or school account)</span></span> | <span data-ttu-id="9f713-126">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9f713-126">Mail.Read</span></span>    |
|<span data-ttu-id="9f713-127">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f713-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f713-128">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9f713-128">Mail.Read</span></span>    |
|<span data-ttu-id="9f713-129">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f713-129">Application</span></span> | <span data-ttu-id="9f713-130">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9f713-130">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f713-131">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f713-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9f713-132">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9f713-132">Optional query parameters</span></span>
<span data-ttu-id="9f713-133">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9f713-133">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9f713-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f713-134">Request headers</span></span>
| <span data-ttu-id="9f713-135">Name</span><span class="sxs-lookup"><span data-stu-id="9f713-135">Name</span></span>       | <span data-ttu-id="9f713-136">Typ</span><span class="sxs-lookup"><span data-stu-id="9f713-136">Type</span></span> | <span data-ttu-id="9f713-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f713-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9f713-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f713-138">Authorization</span></span>  | <span data-ttu-id="9f713-139">string</span><span class="sxs-lookup"><span data-stu-id="9f713-139">string</span></span>  | <span data-ttu-id="9f713-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f713-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f713-142">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f713-142">Request body</span></span>
<span data-ttu-id="9f713-143">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9f713-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f713-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f713-144">Response</span></span>

<span data-ttu-id="9f713-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f713-145">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9f713-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f713-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f713-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f713-147">Request</span></span>
<span data-ttu-id="9f713-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f713-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="9f713-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f713-149">Response</span></span>
<span data-ttu-id="9f713-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f713-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "html",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

## <a name="see-also"></a><span data-ttu-id="9f713-153">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="9f713-153">See also</span></span>

- [<span data-ttu-id="9f713-154">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="9f713-154">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="9f713-155">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="9f713-155">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
