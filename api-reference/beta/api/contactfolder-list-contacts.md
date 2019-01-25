---
title: Kontakte auflisten
description: Rufen Sie alle Kontakte im Postfach des angemeldeten Benutzers (.../me/contacts) oder aus der angegebenen Kontaktordner.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b3e5ee2ad13e454c0ab118b1a5b14509c9b33fbd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529208"
---
# <a name="list-contacts"></a><span data-ttu-id="69775-103">Kontakte auflisten</span><span class="sxs-lookup"><span data-stu-id="69775-103">List contacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69775-104">Rufen Sie alle Kontakte im Postfach des angemeldeten Benutzers (.../me/contacts) oder aus der angegebenen Kontaktordner.</span><span class="sxs-lookup"><span data-stu-id="69775-104">Get all the contacts in the signed-in user's mailbox (.../me/contacts), or from the specified contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="69775-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="69775-105">Permissions</span></span>
<span data-ttu-id="69775-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69775-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69775-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="69775-108">Permission type</span></span>      | <span data-ttu-id="69775-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="69775-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69775-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="69775-110">Delegated (work or school account)</span></span> | <span data-ttu-id="69775-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69775-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="69775-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="69775-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69775-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69775-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="69775-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="69775-114">Application</span></span> | <span data-ttu-id="69775-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69775-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="69775-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="69775-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="69775-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="69775-117">Optional query parameters</span></span>
<span data-ttu-id="69775-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="69775-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="69775-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="69775-119">Request headers</span></span>
| <span data-ttu-id="69775-120">Name</span><span class="sxs-lookup"><span data-stu-id="69775-120">Name</span></span>       | <span data-ttu-id="69775-121">Typ</span><span class="sxs-lookup"><span data-stu-id="69775-121">Type</span></span> | <span data-ttu-id="69775-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69775-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="69775-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="69775-123">Authorization</span></span>  | <span data-ttu-id="69775-124">string</span><span class="sxs-lookup"><span data-stu-id="69775-124">string</span></span>  | <span data-ttu-id="69775-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="69775-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69775-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="69775-127">Request body</span></span>
<span data-ttu-id="69775-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="69775-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69775-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="69775-129">Response</span></span>

<span data-ttu-id="69775-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Contact](../resources/contact.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="69775-130">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="69775-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="69775-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69775-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="69775-132">Request</span></span>
<span data-ttu-id="69775-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="69775-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
```
##### <a name="response"></a><span data-ttu-id="69775-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="69775-134">Response</span></span>
<span data-ttu-id="69775-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="69775-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "birthday": "2016-10-19T10:37:00Z",
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
<!--
{
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-list-contacts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
