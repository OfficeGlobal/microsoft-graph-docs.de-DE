---
title: plannerPlan erstellen
description: Verwenden Sie diese API zum Erstellen eines neuen **plannerPlan**-Objekts.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: a5383bacedef2e7e6df718a4286f034e67f6a7d9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524716"
---
# <a name="create-plannerplan"></a><span data-ttu-id="f3414-103">plannerPlan erstellen</span><span class="sxs-lookup"><span data-stu-id="f3414-103">Create plannerPlan</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3414-104">Verwenden Sie diese API zum Erstellen eines neuen **plannerPlan**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f3414-104">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3414-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f3414-105">Permissions</span></span>

<span data-ttu-id="f3414-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3414-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f3414-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f3414-108">Permission type</span></span>                        | <span data-ttu-id="f3414-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f3414-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f3414-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f3414-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f3414-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3414-111">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="f3414-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f3414-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3414-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3414-113">Not supported.</span></span>                              |
| <span data-ttu-id="f3414-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f3414-114">Application</span></span>                            | <span data-ttu-id="f3414-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3414-115">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="f3414-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3414-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
``` http
POST /planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="f3414-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f3414-117">Request headers</span></span>

| <span data-ttu-id="f3414-118">Name</span><span class="sxs-lookup"><span data-stu-id="f3414-118">Name</span></span>          | <span data-ttu-id="f3414-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3414-119">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f3414-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3414-120">Authorization</span></span> | <span data-ttu-id="f3414-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f3414-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3414-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f3414-123">Request body</span></span>

<span data-ttu-id="f3414-p103">Geben Sie im Anforderungstext eine JSON-Darstellung des [plannerPlan](../resources/plannerplan.md)-Objekts an. Die Eigenschaft „owner“ des **plannerPlan**-Objekts muss auf die ID eines [group](../resources/group.md)-Objekts festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="f3414-p103">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

><span data-ttu-id="f3414-126">**Hinweis:** Der Benutzer, der den Plan erstellen wird, muss ein Mitglied der Gruppe, die Besitzer des Plans.</span><span class="sxs-lookup"><span data-stu-id="f3414-126">**Note:** The user who is creating the plan must be a member of the group that will own the plan.</span></span> <span data-ttu-id="f3414-127">Wenn Sie eine neue Gruppe erstellen, mit der [Gruppe erstellen](../api/group-post-groups.md), werden Sie nicht als Mitglied der Gruppe hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f3414-127">When you create a new group by using [Create group](../api/group-post-groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="f3414-128">Nach dem Erstellen der Gruppe fügen selbst mithilfe der [Gruppe Mitglieder buchen](../api/group-post-members.md)als Mitglied hinzu.</span><span class="sxs-lookup"><span data-stu-id="f3414-128">After the group is created, add yourself as a member by using [group post members](../api/group-post-members.md).</span></span>

## <a name="response"></a><span data-ttu-id="f3414-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3414-129">Response</span></span>

<span data-ttu-id="f3414-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [plannerPlan](../resources/plannerplan.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3414-130">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="f3414-p105">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="f3414-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="f3414-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f3414-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3414-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3414-135">Request</span></span>

<span data-ttu-id="f3414-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f3414-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_planner"
}-->
``` http
POST https://graph.microsoft.com/beta/planner/plans
Content-type: application/json
Content-length: 381

{
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value"
}
```

<span data-ttu-id="f3414-137">Geben Sie im Anforderungstext eine JSON-Darstellung des [plannerPlan](../resources/plannerplan.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f3414-137">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="f3414-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3414-138">Response</span></span>

<span data-ttu-id="f3414-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3414-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planner-post-plans.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
