---
title: Kontakt abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Kontaktobjekts abrufen.
author: angelgolfer-ms
ms.openlocfilehash: 20677bd9cf10f1098ff233a8f60d69e7728aab85
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331486"
---
# <a name="get-contact"></a><span data-ttu-id="d9db1-103">Kontakt abrufen</span><span class="sxs-lookup"><span data-stu-id="d9db1-103">Get contact</span></span>

<span data-ttu-id="d9db1-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Kontaktobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="d9db1-104">Retrieve the properties and relationships of a contact object.</span></span>

<span data-ttu-id="d9db1-105">Es gibt zwei Szenarien, eine app auf einen Kontakt in einen anderen Benutzer Kontaktordner abrufen können:</span><span class="sxs-lookup"><span data-stu-id="d9db1-105">There are two scenarios where an app can get a contact in another user's contact folder:</span></span>

* <span data-ttu-id="d9db1-106">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="d9db1-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="d9db1-107">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer diesen Benutzer einen Kontaktordner freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="d9db1-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="d9db1-108">Finden Sie [ausführliche Informationen und ein Beispiel](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="d9db1-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="d9db1-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d9db1-109">Permissions</span></span>
<span data-ttu-id="d9db1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9db1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9db1-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d9db1-112">Permission type</span></span>      | <span data-ttu-id="d9db1-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d9db1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9db1-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d9db1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d9db1-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9db1-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d9db1-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d9db1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9db1-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9db1-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d9db1-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d9db1-118">Application</span></span> | <span data-ttu-id="d9db1-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9db1-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9db1-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9db1-120">HTTP request</span></span>
<span data-ttu-id="d9db1-121"><!-- { "blockType": "ignored" } -->[Wenden Sie sich](../resources/contact.md) von einem Benutzer standardmäßig [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="d9db1-121"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="d9db1-122">Ein [Kontakt](../resources/contact.md) aus dem [contactFolder](../resources/contactfolder.md) oberster Ebene eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d9db1-122">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="d9db1-p103">Ein [Kontakt](../resources/contact.md) in einem untergeordneten Ordner eines [contactFolder](../resources/mailfolder.md). Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber ein Kontakt kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="d9db1-p103">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d9db1-125">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d9db1-125">Optional query parameters</span></span>
|<span data-ttu-id="d9db1-126">Name</span><span class="sxs-lookup"><span data-stu-id="d9db1-126">Name</span></span>|<span data-ttu-id="d9db1-127">Wert</span><span class="sxs-lookup"><span data-stu-id="d9db1-127">Value</span></span>|<span data-ttu-id="d9db1-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d9db1-128">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="d9db1-129">$expand</span><span class="sxs-lookup"><span data-stu-id="d9db1-129">$expand</span></span>|<span data-ttu-id="d9db1-130">string</span><span class="sxs-lookup"><span data-stu-id="d9db1-130">string</span></span>|<span data-ttu-id="d9db1-p104">Durch Trennzeichen getrennte Liste der Beziehungen, die in der Antwort erweitert und aufgenommen werden. Unterstützte Namen finden Sie in der Beziehungstabelle des [contact](../resources/contact.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d9db1-p104">Comma-separated list of relationships to expand and include in the response. See the relationships table of the [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="d9db1-133">$select</span><span class="sxs-lookup"><span data-stu-id="d9db1-133">$select</span></span>|<span data-ttu-id="d9db1-134">string</span><span class="sxs-lookup"><span data-stu-id="d9db1-134">string</span></span>|<span data-ttu-id="d9db1-135">Durch Trennzeichen getrennte Liste der Eigenschaften, die in der Antwort aufgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="d9db1-135">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="d9db1-136">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d9db1-136">Request headers</span></span>
| <span data-ttu-id="d9db1-137">Header</span><span class="sxs-lookup"><span data-stu-id="d9db1-137">Header</span></span>       | <span data-ttu-id="d9db1-138">Wert</span><span class="sxs-lookup"><span data-stu-id="d9db1-138">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d9db1-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9db1-139">Authorization</span></span>  | <span data-ttu-id="d9db1-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d9db1-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d9db1-142">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d9db1-142">Request body</span></span>
<span data-ttu-id="d9db1-143">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d9db1-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9db1-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9db1-144">Response</span></span>

<span data-ttu-id="d9db1-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [contact](../resources/contact.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9db1-145">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d9db1-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d9db1-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9db1-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9db1-147">Request</span></span>
<span data-ttu-id="d9db1-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d9db1-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="d9db1-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9db1-149">Response</span></span>
<span data-ttu-id="d9db1-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9db1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "businessHomePage": "https://www.contoso.com",
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
