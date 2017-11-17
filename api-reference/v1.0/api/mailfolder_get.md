# <a name="get-mailfolder"></a><span data-ttu-id="4aace-101">mailFolder abrufen</span><span class="sxs-lookup"><span data-stu-id="4aace-101">Get mailFolder</span></span>

<span data-ttu-id="4aace-102">Mit dieser Methode können Sie die Eigenschaften und Beziehungen eines Nachrichtenordnerobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="4aace-102">Retrieve the properties and relationships of a message object.</span></span>


### <a name="get-another-users-message-folder"></a><span data-ttu-id="4aace-103">Anzeigen von Nachrichtenordnern eines anderen Benutzers</span><span class="sxs-lookup"><span data-stu-id="4aace-103">Get another user's contact folder</span></span>

<span data-ttu-id="4aace-104">Wenn Sie über Anwendungsberechtigungen oder die entsprechenden delegierten [Berechtigungen](#permissions) eines Benutzers verfügen, können Sie den Nachrichtenordner eines anderen Benutzers anzeigen.</span><span class="sxs-lookup"><span data-stu-id="4aace-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to a get contact folder of another user's.</span></span> <span data-ttu-id="4aace-105">Dieser Abschnitt enthält Szenarien zu delegierten Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="4aace-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="4aace-106">Beispiel: Ihre App besitzt delegierte Berechtigungen des Benutzers John.</span><span class="sxs-lookup"><span data-stu-id="4aace-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="4aace-107">Der Benutzer Garth hat einen Nachrichtenordner für John freigegeben.</span><span class="sxs-lookup"><span data-stu-id="4aace-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="4aace-108">Sie können den freigegebenen Ordner aufrufen, indem Sie Garths Benutzer-ID (oder den Benutzerprinzipalnamen) in der unten gezeigten Beispielabfrage angeben.</span><span class="sxs-lookup"><span data-stu-id="4aace-108">You can get that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/mailFolders/{id}
```

<span data-ttu-id="4aace-109">Diese Funktion gilt für alle unterstützten GET-Nachrichtenordnervorgänge für einen einzelnen Benutzer (siehe Abschnitt [HTTP-Anforderung](#http-request) unten).</span><span class="sxs-lookup"><span data-stu-id="4aace-109">This capability applies to all GET contact folder operations for an individual user, as described in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="4aace-110">Sie gilt auch, wenn Garth sein gesamtes Postfach an John delegiert hat.</span><span class="sxs-lookup"><span data-stu-id="4aace-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="4aace-111">Wenn Garth weder seinen Nachrichtenordner für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4aace-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="4aace-112">In solchen Fällen funktioniert die Angabe einer Benutzer-ID oder eines Benutzerprinzipalnamens nur, um den Nachrichtenordner eines angemeldeten Benutzers abzurufen, und die Abfrage entspricht der Verwendung der Verknüpfung the /me:</span><span class="sxs-lookup"><span data-stu-id="4aace-112">In such cases, specifying a user ID or user principal name only works for getting a contact folder of the signed-in user’s, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
```

<span data-ttu-id="4aace-113">Diese Funktion ist nur in GET-Vorgängen verfügbar für:</span><span class="sxs-lookup"><span data-stu-id="4aace-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="4aace-114">Freigegebene Kontaktordner, Kalender und Nachrichtenordner</span><span class="sxs-lookup"><span data-stu-id="4aace-114">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="4aace-115">Kontakte, Ereignisse und Nachrichten in freigegebenen Ordnern</span><span class="sxs-lookup"><span data-stu-id="4aace-115">Contacts and events in shared folders</span></span>
- <span data-ttu-id="4aace-116">Die oben aufgeführten Ressourcen in delegierten Postfächern</span><span class="sxs-lookup"><span data-stu-id="4aace-116">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="4aace-117">Diese Funktion steht in anderen Vorgängen für Kontakte, Ereignisse, Nachrichten und deren Ordner nicht zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="4aace-117">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="4aace-118">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4aace-118">Permissions</span></span>
<span data-ttu-id="4aace-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4aace-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4aace-121">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4aace-121">Permission type</span></span>      | <span data-ttu-id="4aace-122">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4aace-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4aace-123">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4aace-123">Delegated (work or school account)</span></span> | <span data-ttu-id="4aace-124">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4aace-124">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4aace-125">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4aace-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4aace-126">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4aace-126">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4aace-127">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4aace-127">Application</span></span> | <span data-ttu-id="4aace-128">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4aace-128">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4aace-129">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4aace-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4aace-130">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4aace-130">Optional query parameters</span></span>
<span data-ttu-id="4aace-131">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4aace-131">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4aace-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4aace-132">Request headers</span></span>
| <span data-ttu-id="4aace-133">Name</span><span class="sxs-lookup"><span data-stu-id="4aace-133">Name</span></span>       | <span data-ttu-id="4aace-134">Typ</span><span class="sxs-lookup"><span data-stu-id="4aace-134">Type</span></span> | <span data-ttu-id="4aace-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4aace-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4aace-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="4aace-136">Authorization</span></span>  | <span data-ttu-id="4aace-137">string</span><span class="sxs-lookup"><span data-stu-id="4aace-137">string</span></span>  | <span data-ttu-id="4aace-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4aace-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4aace-140">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4aace-140">Request body</span></span>
<span data-ttu-id="4aace-141">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4aace-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4aace-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="4aace-142">Response</span></span>

<span data-ttu-id="4aace-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [MailFolder](../resources/mailfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4aace-143">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4aace-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4aace-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4aace-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4aace-145">Request</span></span>
<span data-ttu-id="4aace-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4aace-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="4aace-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="4aace-147">Response</span></span>
<span data-ttu-id="4aace-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4aace-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
