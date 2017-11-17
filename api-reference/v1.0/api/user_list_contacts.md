# <a name="list-contacts"></a><span data-ttu-id="e46c0-101">Kontakte auflisten</span><span class="sxs-lookup"><span data-stu-id="e46c0-101">List contacts</span></span>

<span data-ttu-id="e46c0-102">Mit dieser API können Sie eine Kontaktsammlung aus dem Standardkontaktordner des angemeldeten Benutzers abrufen.</span><span class="sxs-lookup"><span data-stu-id="e46c0-102">Get a contact collection from the default Contacts folder of the signed-in user.</span></span>


### <a name="get-contacts-in-another-users-contact-folder"></a><span data-ttu-id="e46c0-103">Abrufen von Kontakten aus dem Kontaktordner eines anderen Benutzers</span><span class="sxs-lookup"><span data-stu-id="e46c0-103">Get contacts in another user's contact folder</span></span>

<span data-ttu-id="e46c0-104">Wenn Sie über Anwendungsberechtigungen oder die entsprechenden delegierten [Berechtigungen](#permissions) eines Benutzers verfügen, können Sie Kontakte aus dem Kontaktordner eines anderen Benutzers anzeigen.</span><span class="sxs-lookup"><span data-stu-id="e46c0-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get contacts from another user's contact folder.</span></span> <span data-ttu-id="e46c0-105">Dieser Abschnitt enthält Szenarien zu delegierten Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="e46c0-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="e46c0-106">Beispiel: Ihre App besitzt delegierte Berechtigungen des Benutzers John.</span><span class="sxs-lookup"><span data-stu-id="e46c0-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="e46c0-107">Der Benutzer Garth hat einen Kontaktordner für John freigegeben.</span><span class="sxs-lookup"><span data-stu-id="e46c0-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="e46c0-108">Sie können die Kontakte in diesem freigegebenen Ordner aufrufen, indem Sie Garths Benutzer-ID (oder den Benutzerprinzipalnamen) in der unten gezeigten Beispielabfrage angeben.</span><span class="sxs-lookup"><span data-stu-id="e46c0-108">You can get the contacts in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contacts
```

<span data-ttu-id="e46c0-109">Diese Funktion gilt für alle unterstützten GET-Kontaktvorgänge für einen einzelnen Benutzer (siehe Abschnitt [HTTP-Anforderung](#http-request) unten).</span><span class="sxs-lookup"><span data-stu-id="e46c0-109">This capability applies to all the supported GET contacts operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="e46c0-110">Sie gilt auch, wenn Garth sein gesamtes Postfachs an John delegiert hat.</span><span class="sxs-lookup"><span data-stu-id="e46c0-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="e46c0-111">Wenn Garth weder seinen Kontaktordner für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e46c0-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="e46c0-112">In solchen Fällen funktioniert die Angabe einer Benutzer-ID oder eines Benutzerprinzipalnamens nur, um Kontakte aus dem Kontaktordner eines angemeldeten Benutzers abzurufen, und die Abfrage entspricht der Verwendung der Verknüpfung the /me:</span><span class="sxs-lookup"><span data-stu-id="e46c0-112">In such cases, specifying a user ID or user principal name only works for getting contacts in the signed-in user’s own contact folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
```

<span data-ttu-id="e46c0-113">Diese Funktion ist nur in GET-Vorgängen verfügbar für:</span><span class="sxs-lookup"><span data-stu-id="e46c0-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="e46c0-114">Freigegebene Kontaktordner, Kalender und Nachrichtenordner</span><span class="sxs-lookup"><span data-stu-id="e46c0-114">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="e46c0-115">Kontakte, Ereignisse und Nachrichten in freigegebenen Ordnern</span><span class="sxs-lookup"><span data-stu-id="e46c0-115">Contacts and events in shared folders</span></span>
- <span data-ttu-id="e46c0-116">Die oben aufgeführten Ressourcen in delegierten Postfächern</span><span class="sxs-lookup"><span data-stu-id="e46c0-116">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="e46c0-117">Diese Funktion steht in anderen Vorgängen für Kontakte, Ereignisse, Nachrichten und deren Ordner nicht zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="e46c0-117">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="e46c0-118">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e46c0-118">Permissions</span></span>
<span data-ttu-id="e46c0-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e46c0-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e46c0-121">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e46c0-121">Permission type</span></span>      | <span data-ttu-id="e46c0-122">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e46c0-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e46c0-123">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e46c0-123">Delegated (work or school account)</span></span> | <span data-ttu-id="e46c0-124">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e46c0-124">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e46c0-125">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e46c0-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e46c0-126">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e46c0-126">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e46c0-127">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e46c0-127">Application</span></span> | <span data-ttu-id="e46c0-128">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e46c0-128">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e46c0-129">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e46c0-129">HTTP request</span></span>

<span data-ttu-id="e46c0-130">So rufen Sie alle Kontakte in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="e46c0-130">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="e46c0-131">So rufen Sie Kontakte in einem spezifischen Ordner in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="e46c0-131">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e46c0-132">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e46c0-132">Optional query parameters</span></span>
<span data-ttu-id="e46c0-133">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e46c0-133">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="e46c0-134">Zum Beispiel können Sie die `$filter` Abfrageparameter verwenden, um Kontakte auf Basis der Domäne mit ihren E-Mail-Adressen filtern:</span><span class="sxs-lookup"><span data-stu-id="e46c0-134">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a><span data-ttu-id="e46c0-135">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e46c0-135">Request headers</span></span>
| <span data-ttu-id="e46c0-136">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e46c0-136">Header</span></span>       | <span data-ttu-id="e46c0-137">Wert</span><span class="sxs-lookup"><span data-stu-id="e46c0-137">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e46c0-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="e46c0-138">Authorization</span></span>  | <span data-ttu-id="e46c0-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e46c0-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e46c0-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e46c0-141">Content-Type</span></span>   | <span data-ttu-id="e46c0-142">application/json</span><span class="sxs-lookup"><span data-stu-id="e46c0-142">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e46c0-143">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e46c0-143">Request body</span></span>
<span data-ttu-id="e46c0-144">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e46c0-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e46c0-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="e46c0-145">Response</span></span>

<span data-ttu-id="e46c0-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Contact](../resources/contact.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e46c0-146">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e46c0-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e46c0-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e46c0-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e46c0-148">Request</span></span>
<span data-ttu-id="e46c0-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e46c0-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="e46c0-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="e46c0-150">Response</span></span>
<span data-ttu-id="e46c0-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e46c0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
