---
title: contactFolders auflisten
description: Rufen Sie die Kontakt Ordner im Postfach des angemeldeten Benutzers.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f5f0a485c3c134b6627fce5d3b8f04c26dee503e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523281"
---
# <a name="list-contactfolders"></a><span data-ttu-id="274c4-103">contactFolders auflisten</span><span class="sxs-lookup"><span data-stu-id="274c4-103">List contactFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="274c4-104">Rufen Sie die Kontakt Ordner im Postfach des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="274c4-104">Get all the contact folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="274c4-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="274c4-105">Permissions</span></span>
<span data-ttu-id="274c4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="274c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="274c4-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="274c4-108">Permission type</span></span>      | <span data-ttu-id="274c4-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="274c4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="274c4-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="274c4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="274c4-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="274c4-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="274c4-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="274c4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="274c4-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="274c4-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="274c4-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="274c4-114">Application</span></span> | <span data-ttu-id="274c4-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="274c4-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="274c4-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="274c4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="274c4-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="274c4-117">Optional query parameters</span></span>
<span data-ttu-id="274c4-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="274c4-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="274c4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="274c4-119">Request headers</span></span>
| <span data-ttu-id="274c4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="274c4-120">Header</span></span>       | <span data-ttu-id="274c4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="274c4-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="274c4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="274c4-122">Authorization</span></span>  | <span data-ttu-id="274c4-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="274c4-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="274c4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="274c4-125">Content-Type</span></span>   | <span data-ttu-id="274c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="274c4-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="274c4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="274c4-127">Request body</span></span>
<span data-ttu-id="274c4-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="274c4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="274c4-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="274c4-129">Response</span></span>

<span data-ttu-id="274c4-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [ContactFolder](../resources/contactfolder.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="274c4-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="274c4-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="274c4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="274c4-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="274c4-132">Request</span></span>
<span data-ttu-id="274c4-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="274c4-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders
```
##### <a name="response"></a><span data-ttu-id="274c4-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="274c4-134">Response</span></span>
<span data-ttu-id="274c4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="274c4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "wellKnownName": "wellKnownName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-contactfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
