# <a name="get-contact"></a><span data-ttu-id="d7fd1-101">Kontakt abrufen</span><span class="sxs-lookup"><span data-stu-id="d7fd1-101">Get contact</span></span>

<span data-ttu-id="d7fd1-102">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Kontaktobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-102">Retrieve the properties and relationships of a contact object.</span></span>


### <a name="get-contacts-in-another-users-contact-folder"></a><span data-ttu-id="d7fd1-103">Abrufen von Kontakten aus dem Kontaktordner eines anderen Benutzers</span><span class="sxs-lookup"><span data-stu-id="d7fd1-103">Get contacts in another user's contact folder</span></span>

<span data-ttu-id="d7fd1-104">Wenn Sie über Anwendungsberechtigungen oder die entsprechenden delegierten [Berechtigungen](#permissions) eines Benutzers verfügen, können Sie Kontakte aus dem Kontaktordner eines anderen Benutzers anzeigen.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get contacts from another user's contact folder.</span></span> <span data-ttu-id="d7fd1-105">Dieser Abschnitt enthält Szenarien zu delegierten Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="d7fd1-106">Beispiel: Ihre App besitzt delegierte Berechtigungen des Benutzers John.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="d7fd1-107">Der Benutzer Garth hat einen Kontaktordner für John freigegeben.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="d7fd1-108">Sie können einen Kontakt in diesem freigegebenen Ordner aufrufen, indem Sie Garths Benutzer-ID (oder den Benutzerprinzipalnamen) in der unten gezeigten Beispielabfrage angeben.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-108">You can get a contact in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contacts/{id}
```

<span data-ttu-id="d7fd1-109">Diese Funktion gilt für alle unterstützten GET-Kontaktvorgänge für einen einzelnen Benutzer (siehe Abschnitt [HTTP-Anforderung](#http-request) unten).</span><span class="sxs-lookup"><span data-stu-id="d7fd1-109">This capability applies to all the supported GET contacts operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="d7fd1-110">Sie gilt auch, wenn Garth sein gesamtes Postfachs an John delegiert hat.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="d7fd1-111">Wenn Garth weder seinen Kontaktordner für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="d7fd1-112">In solchen Fällen funktioniert die Angabe einer Benutzer-ID oder eines Benutzerprinzipalnamens nur, um einen Kontakt aus dem Kontaktordner eines angemeldeten Benutzers abzurufen, und die Abfrage entspricht der Verwendung der Verknüpfung the /me:</span><span class="sxs-lookup"><span data-stu-id="d7fd1-112">In such cases, specifying a user ID or user principal name only works for getting a contact in the signed-in user’s own contact folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}
```

<span data-ttu-id="d7fd1-113">Diese Funktion ist nur in GET-Vorgängen verfügbar für:</span><span class="sxs-lookup"><span data-stu-id="d7fd1-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="d7fd1-114">Freigegebene Kontaktordner, Kalender und Nachrichtenordner</span><span class="sxs-lookup"><span data-stu-id="d7fd1-114">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="d7fd1-115">Kontakte, Ereignisse und Nachrichten in freigegebenen Ordnern</span><span class="sxs-lookup"><span data-stu-id="d7fd1-115">Contacts and events in shared folders</span></span>
- <span data-ttu-id="d7fd1-116">Die oben aufgeführten Ressourcen in delegierten Postfächern</span><span class="sxs-lookup"><span data-stu-id="d7fd1-116">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="d7fd1-117">Diese Funktion steht in anderen Vorgängen für Kontakte, Ereignisse, Nachrichten und deren Ordner nicht zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-117">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="d7fd1-118">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d7fd1-118">Permissions</span></span>
<span data-ttu-id="d7fd1-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d7fd1-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d7fd1-121">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d7fd1-121">Permission type</span></span>      | <span data-ttu-id="d7fd1-122">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d7fd1-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7fd1-123">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d7fd1-123">Delegated (work or school account)</span></span> | <span data-ttu-id="d7fd1-124">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7fd1-124">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d7fd1-125">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d7fd1-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7fd1-126">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7fd1-126">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d7fd1-127">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d7fd1-127">Application</span></span> | <span data-ttu-id="d7fd1-128">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7fd1-128">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7fd1-129">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7fd1-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d7fd1-130">Ein [Kontakt](../resources/contact.md) aus dem standardmäßigen [contactFolder](../resources/contactfolder.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-130">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="d7fd1-131">Ein [Kontakt](../resources/contact.md) aus dem [contactFolder](../resources/contactfolder.md) oberster Ebene eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-131">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="d7fd1-p106">Ein [Kontakt](../resources/contact.md) in einem untergeordneten Ordner eines [contactFolder](../resources/mailfolder.md). Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber ein Kontakt kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-p106">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d7fd1-134">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d7fd1-134">Optional query parameters</span></span>
|<span data-ttu-id="d7fd1-135">Name</span><span class="sxs-lookup"><span data-stu-id="d7fd1-135">Name</span></span>|<span data-ttu-id="d7fd1-136">Wert</span><span class="sxs-lookup"><span data-stu-id="d7fd1-136">Value</span></span>|<span data-ttu-id="d7fd1-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7fd1-137">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="d7fd1-138">$expand</span><span class="sxs-lookup"><span data-stu-id="d7fd1-138">$expand</span></span>|<span data-ttu-id="d7fd1-139">string</span><span class="sxs-lookup"><span data-stu-id="d7fd1-139">string</span></span>|<span data-ttu-id="d7fd1-p107">Durch Trennzeichen getrennte Liste der Beziehungen, die in der Antwort erweitert und aufgenommen werden. Unterstützte Namen finden Sie in der Beziehungstabelle des [contact](../resources/contact.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-p107">Comma-separated list of relationships to expand and include in the response. See the relationships table of the [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="d7fd1-142">$select</span><span class="sxs-lookup"><span data-stu-id="d7fd1-142">$select</span></span>|<span data-ttu-id="d7fd1-143">string</span><span class="sxs-lookup"><span data-stu-id="d7fd1-143">string</span></span>|<span data-ttu-id="d7fd1-144">Durch Trennzeichen getrennte Liste der Eigenschaften, die in der Antwort aufgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-144">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="d7fd1-145">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d7fd1-145">Request headers</span></span>
| <span data-ttu-id="d7fd1-146">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d7fd1-146">Header</span></span>       | <span data-ttu-id="d7fd1-147">Wert</span><span class="sxs-lookup"><span data-stu-id="d7fd1-147">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d7fd1-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7fd1-148">Authorization</span></span>  | <span data-ttu-id="d7fd1-p108">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-p108">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d7fd1-151">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d7fd1-151">Request body</span></span>
<span data-ttu-id="d7fd1-152">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7fd1-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7fd1-153">Response</span></span>

<span data-ttu-id="d7fd1-154">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [contact](../resources/contact.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-154">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d7fd1-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d7fd1-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7fd1-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7fd1-156">Request</span></span>
<span data-ttu-id="d7fd1-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-157">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="d7fd1-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7fd1-158">Response</span></span>
<span data-ttu-id="d7fd1-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d7fd1-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1977

{
  "id": "AAMkAGI2THk0AAA=",
  "createdDateTime": "2014-10-19T23:08:24Z",
  "lastModifiedDateTime": "2014-10-19T23:08:24Z",
  "changeKey": "EQAAABYAAACd9nJ/tVysQos2hTfspaWRAAADTIa4",
  "categories": [],
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "birthday": "1974-07-22",
  "fileAs": "Fort, Garth",
  "displayName": "Garth Fort",
  "givenName": "Garth",
  "initials": "G.F.",
  "middleName": null,
  "nickName": "Garth",
  "surname": "Fort",
  "title": null,
  "yomiGivenName": null,
  "yomiSurname": null,
  "yomiCompanyName": null,
  "generation": null,
  "emailAddresses": [
    {
      "name": "Garth",
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com"
    }
  ],
  "imAddresses": [
    "sip:garthf@a830edad9050849nda1.onmicrosoft.com"
  ],
  "jobTitle": "Web Marketing Manager",
  "companyName": "Contoso, Inc.",
  "department": "Sales & Marketing",
  "officeLocation": "20/1101",
  "profession": null,
  "businessHomePage": "http://www.contoso.com",
  "assistantName": null,
  "manager": null,
  "homePhones": [],
  "mobilePhone": null,
  "businessPhones": [
    "+1 918 555 0101"
  ],
  "homeAddress": {},
  "businessAddress": {
      "street": "10 Contoso Way",
      "city": "Redmond",
      "state": "WA",
      "countryOrRegion": "USA",
      "postalCode": "98075"  
  },
  "otherAddress": {},
  "spouseName": null,
  "personalNotes": null,
  "children": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
