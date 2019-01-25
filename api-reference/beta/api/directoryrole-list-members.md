---
title: Mitglieder auflisten
description: Dient zum Abrufen einer Liste der Benutzer, die der Verzeichnisrolle zugeordnet sind.  Nur Benutzer können einer Verzeichnisrolle zugewiesen werden.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4365408309a8d87387da76695257207f03bf5ce5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519577"
---
# <a name="list-members"></a><span data-ttu-id="f94cb-104">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="f94cb-104">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f94cb-p102">Dient zum Abrufen einer Liste der Benutzer, die der Verzeichnisrolle zugeordnet sind.  Nur Benutzer können einer Verzeichnisrolle zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="f94cb-p102">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="f94cb-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f94cb-107">Permissions</span></span>
<span data-ttu-id="f94cb-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f94cb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f94cb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f94cb-110">Permission type</span></span>      | <span data-ttu-id="f94cb-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f94cb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f94cb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f94cb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f94cb-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f94cb-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f94cb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f94cb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f94cb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f94cb-115">Not supported.</span></span>    |
|<span data-ttu-id="f94cb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f94cb-116">Application</span></span> | <span data-ttu-id="f94cb-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f94cb-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f94cb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f94cb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f94cb-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f94cb-119">Optional query parameters</span></span>
<span data-ttu-id="f94cb-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f94cb-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f94cb-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f94cb-121">Request headers</span></span>
| <span data-ttu-id="f94cb-122">Name</span><span class="sxs-lookup"><span data-stu-id="f94cb-122">Name</span></span>       | <span data-ttu-id="f94cb-123">Typ</span><span class="sxs-lookup"><span data-stu-id="f94cb-123">Type</span></span> | <span data-ttu-id="f94cb-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f94cb-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f94cb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f94cb-125">Authorization</span></span>  | <span data-ttu-id="f94cb-126">string</span><span class="sxs-lookup"><span data-stu-id="f94cb-126">string</span></span>  | <span data-ttu-id="f94cb-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f94cb-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f94cb-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f94cb-129">Request body</span></span>
<span data-ttu-id="f94cb-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f94cb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f94cb-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f94cb-131">Response</span></span>

<span data-ttu-id="f94cb-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f94cb-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f94cb-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f94cb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f94cb-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f94cb-134">Request</span></span>
<span data-ttu-id="f94cb-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f94cb-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="f94cb-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f94cb-136">Response</span></span>
<span data-ttu-id="f94cb-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f94cb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
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
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-list-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
