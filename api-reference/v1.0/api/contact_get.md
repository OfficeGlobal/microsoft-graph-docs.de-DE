# <a name="get-contact"></a><span data-ttu-id="ce337-101">Kontakt abrufen</span><span class="sxs-lookup"><span data-stu-id="ce337-101">Get contact</span></span>

<span data-ttu-id="ce337-102">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Kontaktobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="ce337-102">Retrieve the properties and relationships of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ce337-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ce337-103">Permissions</span></span>
<span data-ttu-id="ce337-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ce337-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ce337-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ce337-106">Permission type</span></span>      | <span data-ttu-id="ce337-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ce337-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce337-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ce337-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ce337-109">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce337-109">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ce337-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ce337-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce337-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce337-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ce337-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ce337-112">Application</span></span> | <span data-ttu-id="ce337-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce337-113">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce337-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce337-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="ce337-115">Ein [Kontakt](../resources/contact.md) aus dem standardmäßigen [contactFolder](../resources/contactfolder.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="ce337-115">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="ce337-116">Ein [Kontakt](../resources/contact.md) aus dem [contactFolder](../resources/contactfolder.md) oberster Ebene eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="ce337-116">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="ce337-p102">Ein [Kontakt](../resources/contact.md) in einem untergeordneten Ordner eines [contactFolder](../resources/mailfolder.md). Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber ein Kontakt kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="ce337-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ce337-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ce337-119">Optional query parameters</span></span>
|<span data-ttu-id="ce337-120">Name</span><span class="sxs-lookup"><span data-stu-id="ce337-120">Name</span></span>|<span data-ttu-id="ce337-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ce337-121">Value</span></span>|<span data-ttu-id="ce337-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce337-122">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="ce337-123">$expand</span><span class="sxs-lookup"><span data-stu-id="ce337-123">$expand</span></span>|<span data-ttu-id="ce337-124">string</span><span class="sxs-lookup"><span data-stu-id="ce337-124">string</span></span>|<span data-ttu-id="ce337-p103">Durch Trennzeichen getrennte Liste der Beziehungen, die in der Antwort erweitert und aufgenommen werden. Unterstützte Namen finden Sie in der Beziehungstabelle des [contact](../resources/contact.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ce337-p103">Comma-separated list of relationships to expand and include in the response. See the relationships table of the [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="ce337-127">$select</span><span class="sxs-lookup"><span data-stu-id="ce337-127">$select</span></span>|<span data-ttu-id="ce337-128">string</span><span class="sxs-lookup"><span data-stu-id="ce337-128">string</span></span>|<span data-ttu-id="ce337-129">Durch Trennzeichen getrennte Liste der Eigenschaften, die in der Antwort aufgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="ce337-129">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="ce337-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ce337-130">Request headers</span></span>
| <span data-ttu-id="ce337-131">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ce337-131">Header</span></span>       | <span data-ttu-id="ce337-132">Wert</span><span class="sxs-lookup"><span data-stu-id="ce337-132">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ce337-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce337-133">Authorization</span></span>  | <span data-ttu-id="ce337-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ce337-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ce337-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ce337-136">Request body</span></span>
<span data-ttu-id="ce337-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ce337-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce337-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce337-138">Response</span></span>

<span data-ttu-id="ce337-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [contact](../resources/contact.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ce337-139">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ce337-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ce337-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce337-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce337-141">Request</span></span>
<span data-ttu-id="ce337-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ce337-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="ce337-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce337-143">Response</span></span>
<span data-ttu-id="ce337-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ce337-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
