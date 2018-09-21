# <a name="get-contact"></a><span data-ttu-id="1826e-101">Kontakt abrufen</span><span class="sxs-lookup"><span data-stu-id="1826e-101">Get contact</span></span>

<span data-ttu-id="1826e-102">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Kontaktobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="1826e-102">Retrieve the properties and relationships of a contact object.</span></span>

<span data-ttu-id="1826e-103">Es gibt zwei Szenarien, in denen eine App einen Kontakt in dem Kontaktordner eines anderen Benutzers abrufen kann:</span><span class="sxs-lookup"><span data-stu-id="1826e-103">There are two scenarios where an app can get a contact in another user's contact folder:</span></span>

* <span data-ttu-id="1826e-104">Wenn die App über Anwendungsberechtigungen verfügt, oder</span><span class="sxs-lookup"><span data-stu-id="1826e-104">If the app has application permissions, or,</span></span>
* <span data-ttu-id="1826e-105">Wenn die App über die entsprechenden delegierten [Berechtigungen](#permissions) von einem Benutzer verfügt und ein anderer Benutzer einen Kontaktordner für diesen Benutzer freigegeben hat oder delegierten Zugriff auf diesen Benutzer gewährt hat.</span><span class="sxs-lookup"><span data-stu-id="1826e-105">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="1826e-106">Siehe [Details und ein Beispiel](../../../concepts/outlook-get-shared-contacts-folders.md).</span><span class="sxs-lookup"><span data-stu-id="1826e-106">See [details and an example](../../../concepts/outlook-get-shared-contacts-folders.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="1826e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1826e-107">Permissions</span></span>
<span data-ttu-id="1826e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1826e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1826e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1826e-110">Permission type</span></span>      | <span data-ttu-id="1826e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1826e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1826e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1826e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1826e-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1826e-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1826e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1826e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1826e-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1826e-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1826e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1826e-116">Application</span></span> | <span data-ttu-id="1826e-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1826e-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1826e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1826e-118">HTTP request</span></span>
<span data-ttu-id="1826e-119"><!-- { "blockType": "ignored" } --> Ein [Kontakt](../resources/contact.md) aus dem standardmäßigen [contactFolder](../resources/contactfolder.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="1826e-119">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="1826e-120">Ein [Kontakt](../resources/contact.md) aus dem [contactFolder](../resources/contactfolder.md) oberster Ebene eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="1826e-120">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="1826e-p103">Ein [Kontakt](../resources/contact.md) in einem untergeordneten Ordner eines [contactFolder](../resources/mailfolder.md). Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber ein Kontakt kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="1826e-p103">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1826e-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1826e-123">Optional query parameters</span></span>
|<span data-ttu-id="1826e-124">Name</span><span class="sxs-lookup"><span data-stu-id="1826e-124">Name</span></span>|<span data-ttu-id="1826e-125">Wert</span><span class="sxs-lookup"><span data-stu-id="1826e-125">Value</span></span>|<span data-ttu-id="1826e-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1826e-126">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="1826e-127">$expand</span><span class="sxs-lookup"><span data-stu-id="1826e-127">$expand</span></span>|<span data-ttu-id="1826e-128">string</span><span class="sxs-lookup"><span data-stu-id="1826e-128">string</span></span>|<span data-ttu-id="1826e-p104">Durch Trennzeichen getrennte Liste der Beziehungen, die in der Antwort erweitert und aufgenommen werden. Unterstützte Namen finden Sie in der Beziehungstabelle des [contact](../resources/contact.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1826e-p104">Comma-separated list of relationships to expand and include in the response. See the relationships table of the [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="1826e-131">$select</span><span class="sxs-lookup"><span data-stu-id="1826e-131">$select</span></span>|<span data-ttu-id="1826e-132">string</span><span class="sxs-lookup"><span data-stu-id="1826e-132">string</span></span>|<span data-ttu-id="1826e-133">Durch Trennzeichen getrennte Liste der Eigenschaften, die in der Antwort aufgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="1826e-133">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="1826e-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1826e-134">Request headers</span></span>
| <span data-ttu-id="1826e-135">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1826e-135">Header</span></span>       | <span data-ttu-id="1826e-136">Wert</span><span class="sxs-lookup"><span data-stu-id="1826e-136">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1826e-137">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1826e-137">Authorization</span></span>  | <span data-ttu-id="1826e-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1826e-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1826e-140">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1826e-140">Request body</span></span>
<span data-ttu-id="1826e-141">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1826e-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1826e-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="1826e-142">Response</span></span>

<span data-ttu-id="1826e-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [contact](../resources/contact.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1826e-143">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1826e-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1826e-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1826e-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1826e-145">Request</span></span>
<span data-ttu-id="1826e-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1826e-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="1826e-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="1826e-147">Response</span></span>
<span data-ttu-id="1826e-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1826e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
