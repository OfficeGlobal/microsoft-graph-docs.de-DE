---
title: plannerPlan erstellen
description: Verwenden Sie diese API zum Erstellen eines neuen **plannerPlan**-Objekts.
ms.openlocfilehash: bc432bec9b69b40a41b0529c548b073086b8ffff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016685"
---
# <a name="create-plannerplan"></a><span data-ttu-id="22e01-103">plannerPlan erstellen</span><span class="sxs-lookup"><span data-stu-id="22e01-103">Create plannerPlan</span></span>

<span data-ttu-id="22e01-104">Verwenden Sie diese API zum Erstellen eines neuen **plannerPlan**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="22e01-104">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="22e01-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="22e01-105">Permissions</span></span>

<span data-ttu-id="22e01-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22e01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22e01-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="22e01-108">Permission type</span></span>                        | <span data-ttu-id="22e01-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="22e01-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="22e01-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="22e01-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="22e01-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22e01-111">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="22e01-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="22e01-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22e01-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22e01-113">Not supported.</span></span>                              |
| <span data-ttu-id="22e01-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="22e01-114">Application</span></span>                            | <span data-ttu-id="22e01-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22e01-115">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="22e01-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="22e01-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
``` http
POST /planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="22e01-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="22e01-117">Request headers</span></span>

| <span data-ttu-id="22e01-118">Name</span><span class="sxs-lookup"><span data-stu-id="22e01-118">Name</span></span>          | <span data-ttu-id="22e01-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="22e01-119">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="22e01-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="22e01-120">Authorization</span></span> | <span data-ttu-id="22e01-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="22e01-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22e01-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="22e01-123">Request body</span></span>

<span data-ttu-id="22e01-p103">Geben Sie im Anforderungstext eine JSON-Darstellung des [plannerPlan](../resources/plannerplan.md)-Objekts an. Die Eigenschaft „owner“ des **plannerPlan**-Objekts muss auf die ID eines [group](../resources/group.md)-Objekts festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="22e01-p103">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

><span data-ttu-id="22e01-126">**Hinweis:** Der Benutzer, der den Plan erstellen wird, muss ein Mitglied der Gruppe, die Besitzer des Plans.</span><span class="sxs-lookup"><span data-stu-id="22e01-126">**Note:** The user who is creating the plan must be a member of the group that will own the plan.</span></span> <span data-ttu-id="22e01-127">Wenn Sie eine neue Gruppe erstellen, mit der [Gruppe erstellen](../api/group-post-groups.md), werden Sie nicht als Mitglied der Gruppe hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="22e01-127">When you create a new group by using [Create group](../api/group-post-groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="22e01-128">Nach dem Erstellen der Gruppe fügen selbst mithilfe der [Gruppe Mitglieder buchen](../api/group-post-members.md)als Mitglied hinzu.</span><span class="sxs-lookup"><span data-stu-id="22e01-128">After the group is created, add yourself as a member by using [group post members](../api/group-post-members.md).</span></span>


## <a name="response"></a><span data-ttu-id="22e01-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="22e01-129">Response</span></span>

<span data-ttu-id="22e01-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [plannerPlan](../resources/plannerplan.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="22e01-130">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="22e01-p105">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="22e01-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="22e01-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="22e01-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="22e01-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="22e01-135">Request</span></span>

<span data-ttu-id="22e01-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="22e01-136">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_planner"
}-->
``` http
POST https://graph.microsoft.com/v1.0/planner/plans
Content-type: application/json
Content-length: 381

{
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value"
}
```

<span data-ttu-id="22e01-137">Geben Sie im Anforderungstext eine JSON-Darstellung des [plannerPlan](../resources/plannerplan.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="22e01-137">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="22e01-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="22e01-138">Response</span></span>

<span data-ttu-id="22e01-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="22e01-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->