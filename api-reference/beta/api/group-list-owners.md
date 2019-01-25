---
title: Besitzer auflisten
description: Dient zum Abrufen einer Liste der Besitzer der Gruppe. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind, die das Gruppenobjekt ändern können.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 477a8fd2e647d8bdc3babdcb48bccba469912e93
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520949"
---
# <a name="list-owners"></a><span data-ttu-id="ddd1e-104">Besitzer auflisten</span><span class="sxs-lookup"><span data-stu-id="ddd1e-104">List owners</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddd1e-p102">Dient zum Abrufen einer Liste der Besitzer der Gruppe. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind, die das Gruppenobjekt ändern können.</span><span class="sxs-lookup"><span data-stu-id="ddd1e-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddd1e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ddd1e-107">Permissions</span></span>
<span data-ttu-id="ddd1e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddd1e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddd1e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ddd1e-110">Permission type</span></span>      | <span data-ttu-id="ddd1e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ddd1e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddd1e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ddd1e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ddd1e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ddd1e-113">Not supported.</span></span>    |
|<span data-ttu-id="ddd1e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ddd1e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddd1e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ddd1e-115">Not supported.</span></span>    |
|<span data-ttu-id="ddd1e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ddd1e-116">Application</span></span> | <span data-ttu-id="ddd1e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ddd1e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddd1e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ddd1e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ddd1e-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ddd1e-119">Optional query parameters</span></span>
<span data-ttu-id="ddd1e-120">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ddd1e-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddd1e-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ddd1e-121">Request headers</span></span>
| <span data-ttu-id="ddd1e-122">Name</span><span class="sxs-lookup"><span data-stu-id="ddd1e-122">Name</span></span>       | <span data-ttu-id="ddd1e-123">Typ</span><span class="sxs-lookup"><span data-stu-id="ddd1e-123">Type</span></span> | <span data-ttu-id="ddd1e-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ddd1e-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ddd1e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddd1e-125">Authorization</span></span>  | <span data-ttu-id="ddd1e-126">string</span><span class="sxs-lookup"><span data-stu-id="ddd1e-126">string</span></span>  | <span data-ttu-id="ddd1e-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ddd1e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddd1e-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ddd1e-129">Request body</span></span>
<span data-ttu-id="ddd1e-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ddd1e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddd1e-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ddd1e-131">Response</span></span>
<span data-ttu-id="ddd1e-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ddd1e-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddd1e-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ddd1e-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ddd1e-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ddd1e-134">Request</span></span>
<span data-ttu-id="ddd1e-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ddd1e-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="ddd1e-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="ddd1e-136">Response</span></span>
<span data-ttu-id="ddd1e-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ddd1e-137">The following is an example of the response.</span></span>
><span data-ttu-id="ddd1e-138">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="ddd1e-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ddd1e-139">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="ddd1e-139">All the properties will be returned from an actual call.</span></span>
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
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-owners.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
