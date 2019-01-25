---
title: Liste recentPlans
description: Abrufen einer Liste der PlannerPlans kürzlich von einem Benutzer angezeigt. Aktualisieren Sie zuletzt angezeigte Pläne, indem die Ressource PlannerUser aktualisieren.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: b4a8e25a31ceb17f85aef139378fa3e3e9058ab4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528739"
---
# <a name="list-recentplans"></a><span data-ttu-id="6134f-104">Liste recentPlans</span><span class="sxs-lookup"><span data-stu-id="6134f-104">List recentPlans</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6134f-105">Abrufen einer Liste der [PlannerPlans](../resources/plannerplan.md) kürzlich von einem Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="6134f-105">Retrieve a list of [plannerPlans](../resources/plannerplan.md) recently viewed by a user.</span></span> <span data-ttu-id="6134f-106">Sie können die zuletzt angezeigte Pläne durch [Aktualisieren der Ressource PlannerUser](planneruser-update.md)aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="6134f-106">You can update recently viewed plans by [updating the plannerUser resource](planneruser-update.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="6134f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6134f-107">Permissions</span></span>
<span data-ttu-id="6134f-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6134f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6134f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6134f-110">Permission type</span></span>      | <span data-ttu-id="6134f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6134f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6134f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6134f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6134f-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6134f-113">Group.Read.All</span></span>    |
|<span data-ttu-id="6134f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6134f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6134f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6134f-115">Not supported.</span></span>    |
|<span data-ttu-id="6134f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6134f-116">Application</span></span> | <span data-ttu-id="6134f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6134f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6134f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6134f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/recentPlans
GET /users/<id>/planner/recentPlans
```

## <a name="request-headers"></a><span data-ttu-id="6134f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6134f-119">Request headers</span></span>
| <span data-ttu-id="6134f-120">Name</span><span class="sxs-lookup"><span data-stu-id="6134f-120">Name</span></span>      |<span data-ttu-id="6134f-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6134f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6134f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6134f-122">Authorization</span></span>  | <span data-ttu-id="6134f-p104">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6134f-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6134f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6134f-125">Request body</span></span>
<span data-ttu-id="6134f-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6134f-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6134f-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="6134f-127">Response</span></span>
<span data-ttu-id="6134f-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [PlannerPlan](../resources/plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="6134f-128">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6134f-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6134f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6134f-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6134f-130">Request</span></span>
<span data-ttu-id="6134f-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6134f-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_recentplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/recentPlans
```
##### <a name="response"></a><span data-ttu-id="6134f-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="6134f-132">Response</span></span>
<span data-ttu-id="6134f-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6134f-133">The following is an example of the response.</span></span> 

><span data-ttu-id="6134f-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="6134f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtUGxhbiAgQEBAQEBAQEBAQEBAQEBDXCc=\"",
      "createdBy": {
        "user": {
          "id": "dd8a8379-1ac1-4eee-861d-ec15f6fa3611"
        },
        "application": {
          "id": "09abbdfd-ed23-44ee-a2d9-a627aa1c90f3"
        }
      },
      "createdDateTime": "2015-10-14T00:57:28.4698344Z",
      "owner": "eacd01dd-84cc-4c12-bd8a-9a33e5aeed11",
      "title": "Budget Planning (2016)",
      "id": "uZWtCtli30CGoWLIWSat1mQAC0ai"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List recentPlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-list-recentplans.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
