# <a name="list-messages"></a><span data-ttu-id="8aa38-101">Nachrichten auflisten</span><span class="sxs-lookup"><span data-stu-id="8aa38-101">List messages</span></span>

<span data-ttu-id="8aa38-102">Mit dieser Methode können Sie die Nachrichten im Postfach des angemeldeten Benutzers abrufen (einschließlich der Nachrichten aus den Ordnern „Gelöschte Elemente“ und „Clutter“).</span><span class="sxs-lookup"><span data-stu-id="8aa38-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="8aa38-103">Zurzeit gibt dieser Vorgang Nachrichtentext ausschließlich im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="8aa38-103">Currently, this operation returns message bodies in only HTML format.</span></span>


### <a name="get-messages-in-another-users-message-folder"></a><span data-ttu-id="8aa38-104">Anzeigen von Nachrichten im Nachrichtenordner eines anderen Benutzers</span><span class="sxs-lookup"><span data-stu-id="8aa38-104">Get messages in another user's message folder</span></span>

<span data-ttu-id="8aa38-105">Wenn Sie über Anwendungsberechtigungen oder die entsprechenden delegierten [Berechtigungen](#permissions) eines Benutzers verfügen, können Sie Nachrichten aus dem Nachrichtenordner eines anderen Benutzers anzeigen.</span><span class="sxs-lookup"><span data-stu-id="8aa38-105">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get messages from another user's message folder.</span></span> <span data-ttu-id="8aa38-106">Dieser Abschnitt enthält Szenarien zu delegierten Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="8aa38-106">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="8aa38-107">Beispiel: Ihre App besitzt delegierte Berechtigungen des Benutzers John.</span><span class="sxs-lookup"><span data-stu-id="8aa38-107">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="8aa38-108">Der Benutzer Garth hat einen Nachrichtenordner für John freigegeben.</span><span class="sxs-lookup"><span data-stu-id="8aa38-108">Suppose another user, Garth, has shared a message folder with John.</span></span> <span data-ttu-id="8aa38-109">Sie können die Nachrichten in diesem freigegebenen Ordner aufrufen, indem Sie Garths Benutzer-ID (oder den Benutzerprinzipalnamen) in der unten gezeigten Beispielabfrage angeben.</span><span class="sxs-lookup"><span data-stu-id="8aa38-109">You can get the messages in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/messages
```

<span data-ttu-id="8aa38-110">Diese Funktion gilt für alle unterstützten GET-Nachrichtenvorgänge für einen einzelnen Benutzer (siehe Abschnitt [HTTP-Anforderung](#http-request) unten).</span><span class="sxs-lookup"><span data-stu-id="8aa38-110">This capability applies to all the supported GET messages operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="8aa38-111">Sie gilt auch, wenn Garth sein gesamtes Postfach an John delegiert hat.</span><span class="sxs-lookup"><span data-stu-id="8aa38-111">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="8aa38-112">Wenn Garth weder seinen Nachrichtenordner für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8aa38-112">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="8aa38-113">In solchen Fällen funktioniert die Angabe einer Benutzer-ID oder eines Benutzerprinzipalnamens nur, um Nachrichten aus dem Nachrichtenordner eines angemeldeten Benutzers anzuzeigen, und die Abfrage entspricht der Verwendung der Verknüpfung the /me:</span><span class="sxs-lookup"><span data-stu-id="8aa38-113">In such cases, specifying a user ID or user principal name only works for getting messages in the signed-in user’s own message folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
```

<span data-ttu-id="8aa38-114">Diese Funktion ist nur in GET-Vorgängen verfügbar für:</span><span class="sxs-lookup"><span data-stu-id="8aa38-114">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="8aa38-115">Freigegebene Kontaktordner, Kalender und Nachrichtenordner</span><span class="sxs-lookup"><span data-stu-id="8aa38-115">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="8aa38-116">Kontakte, Ereignisse und Nachrichten in freigegebenen Ordnern</span><span class="sxs-lookup"><span data-stu-id="8aa38-116">Contacts, events, and messages in shared folders</span></span>
- <span data-ttu-id="8aa38-117">Die oben aufgeführten Ressourcen in delegierten Postfächern</span><span class="sxs-lookup"><span data-stu-id="8aa38-117">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="8aa38-118">Diese Funktion steht in anderen Vorgängen für Kontakte, Ereignisse, Nachrichten und deren Ordner nicht zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="8aa38-118">This capability is not available in other operations for contacts, events, messages, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="8aa38-119">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8aa38-119">Permissions</span></span>
<span data-ttu-id="8aa38-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8aa38-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8aa38-122">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8aa38-122">Permission type</span></span>      | <span data-ttu-id="8aa38-123">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8aa38-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8aa38-124">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8aa38-124">Delegated (work or school account)</span></span> | <span data-ttu-id="8aa38-125">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8aa38-125">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8aa38-126">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8aa38-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8aa38-127">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8aa38-127">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8aa38-128">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8aa38-128">Application</span></span> | <span data-ttu-id="8aa38-129">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8aa38-129">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8aa38-130">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8aa38-130">HTTP request</span></span>

<span data-ttu-id="8aa38-131">So rufen Sie alle Nachrichten in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="8aa38-131">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="8aa38-132">So rufen Sie Nachrichten in einem spezifischen Ordner in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="8aa38-132">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8aa38-133">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8aa38-133">Optional query parameters</span></span>
<span data-ttu-id="8aa38-134">Diese Methode unterstützt die [OData-Abfrageparameter]((http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters)) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8aa38-134">This method supports the [OData Query Parameters]((http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters)) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8aa38-135">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8aa38-135">Request headers</span></span>
| <span data-ttu-id="8aa38-136">Name</span><span class="sxs-lookup"><span data-stu-id="8aa38-136">Name</span></span>       | <span data-ttu-id="8aa38-137">Typ</span><span class="sxs-lookup"><span data-stu-id="8aa38-137">Type</span></span> | <span data-ttu-id="8aa38-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8aa38-138">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8aa38-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="8aa38-139">Authorization</span></span>  | <span data-ttu-id="8aa38-140">string</span><span class="sxs-lookup"><span data-stu-id="8aa38-140">string</span></span>  | <span data-ttu-id="8aa38-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8aa38-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8aa38-143">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="8aa38-143">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="8aa38-144">string</span><span class="sxs-lookup"><span data-stu-id="8aa38-144">string</span></span> | <span data-ttu-id="8aa38-145">Das Format, in der die **body**- und **uniqueBody**-Eigenschaften zurückgegeben werden sollen.</span><span class="sxs-lookup"><span data-stu-id="8aa38-145">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="8aa38-146">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="8aa38-146">Values can be "text" or "html".</span></span> <span data-ttu-id="8aa38-147">Wenn die Kopfzeile nicht angegeben ist, werden die **body**- und **uniqueBody**-Eigenschaften im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8aa38-147">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="8aa38-148">Optional.</span><span class="sxs-lookup"><span data-stu-id="8aa38-148">Optional.</span></span> |


## <a name="request-body"></a><span data-ttu-id="8aa38-149">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8aa38-149">Request body</span></span>
<span data-ttu-id="8aa38-150">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8aa38-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8aa38-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="8aa38-151">Response</span></span>

<span data-ttu-id="8aa38-152">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Message](../resources/message.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8aa38-152">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="8aa38-153">Die Standardseitengröße für diese Anforderung liegt bei 10 Nachrichten.</span><span class="sxs-lookup"><span data-stu-id="8aa38-153">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="8aa38-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8aa38-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8aa38-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8aa38-155">Request</span></span>
<span data-ttu-id="8aa38-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8aa38-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="8aa38-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="8aa38-157">Response</span></span>
<span data-ttu-id="8aa38-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8aa38-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
