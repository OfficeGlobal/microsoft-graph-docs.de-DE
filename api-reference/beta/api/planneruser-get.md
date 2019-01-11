---
title: Abrufen von plannerUser
description: 'Rufen Sie die Eigenschaften und die Beziehungen eines PlannerUser-Objekts ab. Die zurückgegebenen Eigenschaften des Benutzers bevorzugten Pläne enthalten und zuletzt angezeigte Pläne. '
localization_priority: Normal
ms.openlocfilehash: 1abffddb2ddbefdcd0aaeddedffe94ae8ad605d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810640"
---
# <a name="get-planneruser"></a><span data-ttu-id="fd7d1-104">Abrufen von plannerUser</span><span class="sxs-lookup"><span data-stu-id="fd7d1-104">Get plannerUser</span></span>

> <span data-ttu-id="fd7d1-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fd7d1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd7d1-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fd7d1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd7d1-107">Rufen Sie die Eigenschaften und die Beziehungen eines [PlannerUser](../resources/planneruser.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="fd7d1-107">Retrieve the properties and relationships of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="fd7d1-108">Die zurückgegebenen Eigenschaften des Benutzers bevorzugten Pläne enthalten und zuletzt angezeigte Pläne.</span><span class="sxs-lookup"><span data-stu-id="fd7d1-108">The returned properties include the user's favorite plans and recently viewed plans.</span></span> 
## <a name="permissions"></a><span data-ttu-id="fd7d1-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fd7d1-109">Permissions</span></span>
<span data-ttu-id="fd7d1-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd7d1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd7d1-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd7d1-112">Permission type</span></span>      | <span data-ttu-id="fd7d1-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd7d1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd7d1-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd7d1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="fd7d1-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd7d1-115">Group.Read.All</span></span>    |
|<span data-ttu-id="fd7d1-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd7d1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd7d1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd7d1-117">Not supported.</span></span>    |
|<span data-ttu-id="fd7d1-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd7d1-118">Application</span></span> | <span data-ttu-id="fd7d1-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd7d1-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd7d1-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd7d1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner
GET /users/<id>/planner
```

## <a name="request-headers"></a><span data-ttu-id="fd7d1-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd7d1-121">Request headers</span></span>
| <span data-ttu-id="fd7d1-122">Name</span><span class="sxs-lookup"><span data-stu-id="fd7d1-122">Name</span></span>      |<span data-ttu-id="fd7d1-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd7d1-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fd7d1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd7d1-124">Authorization</span></span>  | <span data-ttu-id="fd7d1-p105">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fd7d1-p105">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd7d1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd7d1-127">Request body</span></span>
<span data-ttu-id="fd7d1-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fd7d1-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fd7d1-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd7d1-129">Response</span></span>
<span data-ttu-id="fd7d1-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [PlannerUser](../resources/planneruser.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="fd7d1-130">If successful, this method returns a `200 OK` response code and a [plannerUser](../resources/planneruser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fd7d1-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd7d1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd7d1-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd7d1-132">Request</span></span>
<span data-ttu-id="fd7d1-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fd7d1-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_planneruser"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner
```
##### <a name="response"></a><span data-ttu-id="fd7d1-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd7d1-134">Response</span></span>
<span data-ttu-id="fd7d1-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fd7d1-135">The following is an example of the response.</span></span> 

><span data-ttu-id="fd7d1-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="fd7d1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
