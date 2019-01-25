---
title: Abrufen von plannerUser
description: 'Rufen Sie die Eigenschaften und die Beziehungen eines PlannerUser-Objekts ab. Die zurückgegebenen Eigenschaften des Benutzers bevorzugten Pläne enthalten und zuletzt angezeigte Pläne. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 0ac20564183c36d26440b4532a39413dff47bfb6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510365"
---
# <a name="get-planneruser"></a><span data-ttu-id="aabf5-104">Abrufen von plannerUser</span><span class="sxs-lookup"><span data-stu-id="aabf5-104">Get plannerUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aabf5-105">Rufen Sie die Eigenschaften und die Beziehungen eines [PlannerUser](../resources/planneruser.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="aabf5-105">Retrieve the properties and relationships of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="aabf5-106">Die zurückgegebenen Eigenschaften des Benutzers bevorzugten Pläne enthalten und zuletzt angezeigte Pläne.</span><span class="sxs-lookup"><span data-stu-id="aabf5-106">The returned properties include the user's favorite plans and recently viewed plans.</span></span> 
## <a name="permissions"></a><span data-ttu-id="aabf5-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aabf5-107">Permissions</span></span>
<span data-ttu-id="aabf5-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aabf5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aabf5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aabf5-110">Permission type</span></span>      | <span data-ttu-id="aabf5-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aabf5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aabf5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aabf5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aabf5-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="aabf5-113">Group.Read.All</span></span>    |
|<span data-ttu-id="aabf5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aabf5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aabf5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aabf5-115">Not supported.</span></span>    |
|<span data-ttu-id="aabf5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aabf5-116">Application</span></span> | <span data-ttu-id="aabf5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aabf5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aabf5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aabf5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner
GET /users/<id>/planner
```

## <a name="request-headers"></a><span data-ttu-id="aabf5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aabf5-119">Request headers</span></span>
| <span data-ttu-id="aabf5-120">Name</span><span class="sxs-lookup"><span data-stu-id="aabf5-120">Name</span></span>      |<span data-ttu-id="aabf5-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aabf5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aabf5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aabf5-122">Authorization</span></span>  | <span data-ttu-id="aabf5-p104">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aabf5-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aabf5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aabf5-125">Request body</span></span>
<span data-ttu-id="aabf5-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="aabf5-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="aabf5-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="aabf5-127">Response</span></span>
<span data-ttu-id="aabf5-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [PlannerUser](../resources/planneruser.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="aabf5-128">If successful, this method returns a `200 OK` response code and a [plannerUser](../resources/planneruser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aabf5-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aabf5-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aabf5-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aabf5-130">Request</span></span>
<span data-ttu-id="aabf5-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aabf5-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_planneruser"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner
```
##### <a name="response"></a><span data-ttu-id="aabf5-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="aabf5-132">Response</span></span>
<span data-ttu-id="aabf5-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aabf5-133">The following is an example of the response.</span></span> 

><span data-ttu-id="aabf5-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="aabf5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "favoritePlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586866870001551087",
      "planTitle": "Next Release Discussion"
    },
    "uZWtCtli30CGoWLIWSat1mQAC0ai": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586888705198093378",
      "planTitle": "Product Support"
    }
  },
  "recentPlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-02T22:49:46.155Z",
      "planTitle": "Next Release Discussion"
    },
    "XYE5pqNJu0uuRC2PM4ZQrmQAF2Pn": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-01T19:39:17.57Z",
      "planTitle": "Success Metrics"
    }
  },
  "id": "-YPnMJRiIUSKFyaVjYEkBWQAAc47"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
