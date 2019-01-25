---
title: Liste Gruppe Mitglied
description: Rufen Sie Gruppen und administrative Einheiten, denen die Gruppe ein direktes Mitglied ist.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: ecf127e7cc4af4aada3d75ef6415a242b0a9411b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517540"
---
# <a name="list-group-memberof"></a><span data-ttu-id="cbe21-103">Liste Gruppe Mitglied</span><span class="sxs-lookup"><span data-stu-id="cbe21-103">List group memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbe21-104">Rufen Sie Gruppen und administrative Einheiten, denen die Gruppe ein direktes Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="cbe21-104">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="cbe21-p101">Dieser Vorgang ist nicht transitiv. Im Gegensatz zum Abrufen der Office 365-Gruppen eines Benutzers werden hier alle Typen von Gruppen zurückgegeben, nicht nur Office 365-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="cbe21-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="cbe21-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cbe21-107">Permissions</span></span>

<span data-ttu-id="cbe21-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbe21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbe21-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cbe21-110">Permission type</span></span>      | <span data-ttu-id="cbe21-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cbe21-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbe21-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cbe21-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cbe21-113">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cbe21-113">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cbe21-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cbe21-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbe21-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cbe21-115">Not supported.</span></span>    |
|<span data-ttu-id="cbe21-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cbe21-116">Application</span></span> | <span data-ttu-id="cbe21-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbe21-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbe21-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cbe21-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cbe21-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cbe21-119">Optional query parameters</span></span>
<span data-ttu-id="cbe21-120">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cbe21-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cbe21-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cbe21-121">Request headers</span></span>
| <span data-ttu-id="cbe21-122">Name</span><span class="sxs-lookup"><span data-stu-id="cbe21-122">Name</span></span>       | <span data-ttu-id="cbe21-123">Typ</span><span class="sxs-lookup"><span data-stu-id="cbe21-123">Type</span></span> | <span data-ttu-id="cbe21-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cbe21-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cbe21-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbe21-125">Authorization</span></span>  | <span data-ttu-id="cbe21-126">string</span><span class="sxs-lookup"><span data-stu-id="cbe21-126">string</span></span>  | <span data-ttu-id="cbe21-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cbe21-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbe21-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cbe21-129">Request body</span></span>
<span data-ttu-id="cbe21-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cbe21-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbe21-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="cbe21-131">Response</span></span>
<span data-ttu-id="cbe21-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cbe21-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbe21-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cbe21-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbe21-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cbe21-134">Request</span></span>

<span data-ttu-id="cbe21-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cbe21-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="cbe21-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="cbe21-136">Response</span></span>

<span data-ttu-id="cbe21-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cbe21-137">The following is an example of the response.</span></span>
><span data-ttu-id="cbe21-138">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="cbe21-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cbe21-139">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="cbe21-139">All the properties will be returned from an actual call.</span></span>
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-memberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
