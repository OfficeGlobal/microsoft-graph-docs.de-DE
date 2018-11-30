---
title: Kontakt erstellen
description: Dient zum Hinzufügen eines Kontakts zum Stammordner der Kontakte oder zum Kontaktendpunkt eines anderen Kontaktordners.
ms.openlocfilehash: dea355a848b2df1715f02c5042d31221ae3e49b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016866"
---
# <a name="create-contact"></a><span data-ttu-id="70107-103">Kontakt erstellen</span><span class="sxs-lookup"><span data-stu-id="70107-103">Create Contact</span></span>

<span data-ttu-id="70107-104">Mit dieser API können Sie dem Stammkontaktordner oder dem Kontaktendpunkt eines anderen Kontaktordners Kontakte hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="70107-104">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="70107-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="70107-105">Permissions</span></span>
<span data-ttu-id="70107-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70107-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70107-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="70107-108">Permission type</span></span>      | <span data-ttu-id="70107-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="70107-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70107-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="70107-110">Delegated (work or school account)</span></span> | <span data-ttu-id="70107-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70107-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="70107-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="70107-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70107-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70107-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="70107-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="70107-114">Application</span></span> | <span data-ttu-id="70107-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70107-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="70107-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="70107-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="70107-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="70107-117">Request headers</span></span>
| <span data-ttu-id="70107-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="70107-118">Header</span></span>       | <span data-ttu-id="70107-119">Wert</span><span class="sxs-lookup"><span data-stu-id="70107-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="70107-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="70107-120">Authorization</span></span>  | <span data-ttu-id="70107-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="70107-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="70107-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70107-123">Content-Type</span></span>  | <span data-ttu-id="70107-124">application/json</span><span class="sxs-lookup"><span data-stu-id="70107-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="70107-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="70107-125">Request body</span></span>
<span data-ttu-id="70107-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [Contact](../resources/contact.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="70107-126">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="70107-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="70107-127">Response</span></span>

<span data-ttu-id="70107-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [Contact](../resources/contact.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70107-128">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70107-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="70107-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70107-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="70107-130">Request</span></span>
<span data-ttu-id="70107-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="70107-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contact_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contacts
Content-type: application/json

{
  "givenName": "Pavel",
  "surname": "Bansky",
  "emailAddresses": [
    {
      "address": "pavelb@fabrikam.onmicrosoft.com",
      "name": "Pavel Bansky"
    }
  ],
  "businessPhones": [
    "+1 732 555 0102"
  ]
}
```
<span data-ttu-id="70107-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [contact](../resources/contact.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="70107-132">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="70107-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="70107-133">Response</span></span>
<span data-ttu-id="70107-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70107-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "createdDateTime": "2015-11-09T02:14:32Z",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z",
   "displayName": "Pavel Bansky"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->