---
title: Liste recentPlans
description: Abrufen einer Liste der PlannerPlans kürzlich von einem Benutzer angezeigt. Aktualisieren Sie zuletzt angezeigte Pläne, indem die Ressource PlannerUser aktualisieren.
ms.openlocfilehash: 58c4d786dfdf596df8786db93c32e88b0cf93dfd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064834"
---
# <a name="list-recentplans"></a><span data-ttu-id="944ed-104">Liste recentPlans</span><span class="sxs-lookup"><span data-stu-id="944ed-104">List recentPlans</span></span>

> <span data-ttu-id="944ed-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="944ed-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="944ed-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="944ed-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="944ed-107">Abrufen einer Liste der [PlannerPlans](../resources/plannerplan.md) kürzlich von einem Benutzer angezeigt.</span><span class="sxs-lookup"><span data-stu-id="944ed-107">Retrieve a list of [plannerPlans](../resources/plannerplan.md) recently viewed by a user.</span></span> <span data-ttu-id="944ed-108">Sie können die zuletzt angezeigte Pläne durch [Aktualisieren der Ressource PlannerUser](planneruser-update.md)aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="944ed-108">You can update recently viewed plans by [updating the plannerUser resource](planneruser-update.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="944ed-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="944ed-109">Permissions</span></span>
<span data-ttu-id="944ed-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="944ed-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="944ed-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="944ed-112">Permission type</span></span>      | <span data-ttu-id="944ed-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="944ed-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="944ed-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="944ed-114">Delegated (work or school account)</span></span> | <span data-ttu-id="944ed-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="944ed-115">Group.Read.All</span></span>    |
|<span data-ttu-id="944ed-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="944ed-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="944ed-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="944ed-117">Not supported.</span></span>    |
|<span data-ttu-id="944ed-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="944ed-118">Application</span></span> | <span data-ttu-id="944ed-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="944ed-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="944ed-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="944ed-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/recentPlans
GET /users/<id>/planner/recentPlans
```

## <a name="request-headers"></a><span data-ttu-id="944ed-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="944ed-121">Request headers</span></span>
| <span data-ttu-id="944ed-122">Name</span><span class="sxs-lookup"><span data-stu-id="944ed-122">Name</span></span>      |<span data-ttu-id="944ed-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="944ed-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="944ed-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="944ed-124">Authorization</span></span>  | <span data-ttu-id="944ed-p105">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="944ed-p105">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="944ed-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="944ed-127">Request body</span></span>
<span data-ttu-id="944ed-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="944ed-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="944ed-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="944ed-129">Response</span></span>
<span data-ttu-id="944ed-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [PlannerPlan](../resources/plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="944ed-130">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="944ed-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="944ed-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="944ed-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="944ed-132">Request</span></span>
<span data-ttu-id="944ed-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="944ed-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_recentplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/recentPlans
```
##### <a name="response"></a><span data-ttu-id="944ed-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="944ed-134">Response</span></span>
<span data-ttu-id="944ed-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="944ed-135">The following is an example of the response.</span></span> 

><span data-ttu-id="944ed-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="944ed-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List recentPlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
