# <a name="list-contacts"></a><span data-ttu-id="71814-101">Kontakte auflisten</span><span class="sxs-lookup"><span data-stu-id="71814-101">List contacts</span></span>

<span data-ttu-id="71814-102">Mit dieser API können Sie eine Kontaktsammlung aus dem Standardkontaktordner des angemeldeten Benutzers abrufen.</span><span class="sxs-lookup"><span data-stu-id="71814-102">Get a contact collection from the default Contacts folder of the signed-in user.</span></span>


### <a name="get-contacts-in-another-users-contact-folder"></a><span data-ttu-id="71814-103">Abrufen von Kontakten aus dem Kontaktordner eines anderen Benutzers</span><span class="sxs-lookup"><span data-stu-id="71814-103">Get contacts in another user's contact folder</span></span>

<span data-ttu-id="71814-104">Wenn Sie über Anwendungsberechtigungen oder die entsprechenden delegierten [Berechtigungen](#permissions) eines Benutzers verfügen, können Sie Kontakte aus dem Kontaktordner eines anderen Benutzers anzeigen.</span><span class="sxs-lookup"><span data-stu-id="71814-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get contacts from another user's contact folder.</span></span> <span data-ttu-id="71814-105">Dieser Abschnitt enthält Szenarien zu delegierten Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="71814-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="71814-106">Beispiel: Ihre App besitzt delegierte Berechtigungen des Benutzers John.</span><span class="sxs-lookup"><span data-stu-id="71814-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="71814-107">Der Benutzer Garth hat einen Kontaktordner für John freigegeben.</span><span class="sxs-lookup"><span data-stu-id="71814-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="71814-108">Sie können die Kontakte in diesem freigegebenen Ordner aufrufen, indem Sie Garths Benutzer-ID (oder den Benutzerprinzipalnamen) in der unten gezeigten Beispielabfrage angeben.</span><span class="sxs-lookup"><span data-stu-id="71814-108">You can get the contacts in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contacts
```

<span data-ttu-id="71814-109">Diese Funktion gilt für alle unterstützten GET-Kontaktvorgänge für einen einzelnen Benutzer (siehe Abschnitt [HTTP-Anforderung](#http-request) unten).</span><span class="sxs-lookup"><span data-stu-id="71814-109">This capability applies to all the supported GET contacts operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="71814-110">Sie gilt auch, wenn Garth sein gesamtes Postfachs an John delegiert hat.</span><span class="sxs-lookup"><span data-stu-id="71814-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="71814-111">Wenn Garth weder seinen Kontaktordner für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71814-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="71814-112">In solchen Fällen funktioniert die Angabe einer Benutzer-ID oder eines Benutzerprinzipalnamens nur, um Kontakte aus dem Kontaktordner eines angemeldeten Benutzers abzurufen, und die Abfrage entspricht der Verwendung der Verknüpfung the /me:</span><span class="sxs-lookup"><span data-stu-id="71814-112">In such cases, specifying a user ID or user principal name only works for getting contacts in the signed-in user’s own contact folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
```

<span data-ttu-id="71814-113">Diese Funktion ist nur in GET-Vorgängen verfügbar für:</span><span class="sxs-lookup"><span data-stu-id="71814-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="71814-114">Freigegebene Kontaktordner</span><span class="sxs-lookup"><span data-stu-id="71814-114">Shared contact folders</span></span>
- <span data-ttu-id="71814-115">Freigegebene Kalender</span><span class="sxs-lookup"><span data-stu-id="71814-115">Shared calendars</span></span>
- <span data-ttu-id="71814-116">Kontakte und Ereignisse in freigegebenen Ordnern</span><span class="sxs-lookup"><span data-stu-id="71814-116">Contacts and events in shared folders</span></span>
- <span data-ttu-id="71814-117">Die oben aufgeführten Ressourcen in delegierten Postfächern</span><span class="sxs-lookup"><span data-stu-id="71814-117">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="71814-118">Diese Funktion steht in anderen Vorgängen für Kontakte, Ereignisse und deren Ordner nicht zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="71814-118">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="71814-119">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="71814-119">Permissions</span></span>
<span data-ttu-id="71814-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="71814-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="71814-122">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71814-122">Permission type</span></span>      | <span data-ttu-id="71814-123">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71814-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71814-124">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71814-124">Delegated (work or school account)</span></span> | <span data-ttu-id="71814-125">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71814-125">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="71814-126">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71814-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71814-127">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71814-127">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="71814-128">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71814-128">Application</span></span> | <span data-ttu-id="71814-129">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71814-129">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="71814-130">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71814-130">HTTP request</span></span>

<span data-ttu-id="71814-131">So rufen Sie alle Kontakte in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="71814-131">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="71814-132">So rufen Sie Kontakte in einem spezifischen Ordner in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="71814-132">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="71814-133">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="71814-133">Optional query parameters</span></span>
<span data-ttu-id="71814-134">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="71814-134">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="71814-135">Zum Beispiel können Sie die `$filter` Abfrageparameter verwenden, um Kontakte auf Basis der Domäne mit ihren E-Mail-Adressen filtern:</span><span class="sxs-lookup"><span data-stu-id="71814-135">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a><span data-ttu-id="71814-136">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71814-136">Request headers</span></span>
| <span data-ttu-id="71814-137">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="71814-137">Header</span></span>       | <span data-ttu-id="71814-138">Wert</span><span class="sxs-lookup"><span data-stu-id="71814-138">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="71814-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="71814-139">Authorization</span></span>  | <span data-ttu-id="71814-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="71814-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="71814-142">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71814-142">Content-Type</span></span>   | <span data-ttu-id="71814-143">application/json</span><span class="sxs-lookup"><span data-stu-id="71814-143">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71814-144">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71814-144">Request body</span></span>
<span data-ttu-id="71814-145">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="71814-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71814-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="71814-146">Response</span></span>

<span data-ttu-id="71814-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Contact](../resources/contact.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71814-147">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71814-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71814-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71814-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71814-149">Request</span></span>
<span data-ttu-id="71814-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71814-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="71814-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="71814-151">Response</span></span>
<span data-ttu-id="71814-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71814-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
