---
title: Kontakt erstellen
description: Dient zum Hinzufügen eines Kontakts zum Stammordner der Kontakte oder zum Kontaktendpunkt eines anderen Kontaktordners.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b443a522d4f821861191bcbe7deeff2b6063b236
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967896"
---
# <a name="create-contact"></a><span data-ttu-id="6ee4d-103">Kontakt erstellen</span><span class="sxs-lookup"><span data-stu-id="6ee4d-103">Create Contact</span></span>

> <span data-ttu-id="6ee4d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ee4d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ee4d-106">Mit dieser API können Sie dem Stammkontaktordner oder dem Kontaktendpunkt eines anderen Kontaktordners Kontakte hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-106">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="6ee4d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6ee4d-107">Permissions</span></span>
<span data-ttu-id="6ee4d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ee4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ee4d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6ee4d-110">Permission type</span></span>      | <span data-ttu-id="6ee4d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6ee4d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ee4d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6ee4d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6ee4d-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ee4d-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6ee4d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6ee4d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ee4d-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ee4d-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6ee4d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6ee4d-116">Application</span></span> | <span data-ttu-id="6ee4d-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ee4d-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ee4d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6ee4d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="6ee4d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6ee4d-119">Request headers</span></span>
| <span data-ttu-id="6ee4d-120">Header</span><span class="sxs-lookup"><span data-stu-id="6ee4d-120">Header</span></span>       | <span data-ttu-id="6ee4d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6ee4d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6ee4d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ee4d-122">Authorization</span></span>  | <span data-ttu-id="6ee4d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6ee4d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6ee4d-125">Content-Type</span></span>  | <span data-ttu-id="6ee4d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ee4d-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6ee4d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6ee4d-127">Request body</span></span>
<span data-ttu-id="6ee4d-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [contact](../resources/contact.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-128">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6ee4d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6ee4d-129">Response</span></span>

<span data-ttu-id="6ee4d-130">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code, und [wenden Sie sich](../resources/contact.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-130">If successful, this method returns `201 Created` response code and [contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ee4d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6ee4d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ee4d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6ee4d-132">Request</span></span>
<span data-ttu-id="6ee4d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contact_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/contacts
Content-type: application/json

{
  "givenName": "Pavel",
  "surname": "Bansky",
  "emailAddresses": [
    {
      "address": "pavelb@contoso.onmicrosoft.com",
      "name": "Pavel Bansky",
      "type": "personal"
    },
    {
      "address": "pavelb@fabrikam.onmicrosoft.com",
      "name": "Pavel Bansky",
      "type": "other",
      "otherLabel": "Volunteer work"
    }
  ],
  "phones" : [
    {
      "number": "+1 732 555 0102",
      "type": "business"
    }
  ]
}
```
<span data-ttu-id="6ee4d-134">Geben Sie im Anforderungstext eine JSON-Darstellung des [contact](../resources/contact.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-134">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="6ee4d-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="6ee4d-135">Response</span></span>
<span data-ttu-id="6ee4d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6ee4d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts/$entity",
    "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fW\"",
    "id":"AAMkADh6v5AAAvgTCEAAA=",
    "createdDateTime":"2018-06-11T19:56:07Z",
    "lastModifiedDateTime":"2018-06-11T19:56:07Z",
    "changeKey":"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fW",
    "categories":[

    ],
    "parentFolderId":"AAMkADh6v5AAAAAAEOAAA=",
    "birthday":null,
    "fileAs":"",
    "displayName":"Pavel Bansky",
    "givenName":"Pavel",
    "initials":null,
    "middleName":null,
    "nickName":null,
    "surname":"Bansky",
    "title":null,
    "yomiGivenName":null,
    "yomiSurname":null,
    "yomiCompanyName":null,
    "generation":null,
    "imAddresses":[

    ],
    "jobTitle":null,
    "companyName":null,
    "department":null,
    "officeLocation":null,
    "profession":null,
    "assistantName":null,
    "manager":null,
    "spouseName":null,
    "personalNotes":"",
    "children":[

    ],
    "gender":null,
    "isFavorite":null,
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@contoso.onmicrosoft.com"
        },
        {
            "otherLabel": "Volunteer work",
            "type":"other",
            "name":"Pavel Bansky",
            "address":"pavelb@fabrikam.onmicrosoft.com"
        }
    ],
    "websites":[

    ],
    "phones":[
        {
            "type":"business",
            "number":"+1 732 555 0102"
        }
    ],
    "postalAddresses":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

## <a name="see-also"></a><span data-ttu-id="6ee4d-139">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="6ee4d-139">See also</span></span>

- [<span data-ttu-id="6ee4d-140">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="6ee4d-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="6ee4d-141">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="6ee4d-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
