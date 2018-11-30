---
title: 'GroupLifecyclePolicy: RenewGroup'
description: Verlängert den Ablaufzeitraum einer Gruppe. Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind.
ms.openlocfilehash: 13e1713d3d00e7feac0b23eae8a314e55341e20e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060925"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="ae7f2-104">GroupLifecyclePolicy: RenewGroup</span><span class="sxs-lookup"><span data-stu-id="ae7f2-104">groupLifecyclePolicy: renewGroup</span></span>

> <span data-ttu-id="ae7f2-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ae7f2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae7f2-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae7f2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae7f2-107">Verlängert den Ablaufzeitraum einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="ae7f2-107">Renews a group's expiration.</span></span> <span data-ttu-id="ae7f2-108">Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind.</span><span class="sxs-lookup"><span data-stu-id="ae7f2-108">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="ae7f2-109">**Hinweis:** In v1. 0, [Verwenden Sie die Gruppenressource um Anfragen erneuern zu machen](/graph/api/group-renew?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="ae7f2-109">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="ae7f2-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ae7f2-110">Permissions</span></span>

<span data-ttu-id="ae7f2-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae7f2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="ae7f2-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ae7f2-113">Permission type</span></span>      | <span data-ttu-id="ae7f2-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ae7f2-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae7f2-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae7f2-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ae7f2-116">Group.ReadWrite.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae7f2-116">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="ae7f2-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae7f2-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae7f2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae7f2-118">Not supported</span></span> |
|<span data-ttu-id="ae7f2-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ae7f2-119">Application</span></span> | <span data-ttu-id="ae7f2-120">Group.ReadWrite.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae7f2-120">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae7f2-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae7f2-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="ae7f2-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae7f2-122">Request headers</span></span>

| <span data-ttu-id="ae7f2-123">Name</span><span class="sxs-lookup"><span data-stu-id="ae7f2-123">Name</span></span> | <span data-ttu-id="ae7f2-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae7f2-124">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ae7f2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae7f2-125">Authorization</span></span> | <span data-ttu-id="ae7f2-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae7f2-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae7f2-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae7f2-128">Content-Type</span></span>  | <span data-ttu-id="ae7f2-129">application/json</span><span class="sxs-lookup"><span data-stu-id="ae7f2-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae7f2-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ae7f2-130">Request body</span></span>
<span data-ttu-id="ae7f2-131">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="ae7f2-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ae7f2-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="ae7f2-132">Parameter</span></span> | <span data-ttu-id="ae7f2-133">Typ</span><span class="sxs-lookup"><span data-stu-id="ae7f2-133">Type</span></span> | <span data-ttu-id="ae7f2-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae7f2-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ae7f2-135">groupId</span><span class="sxs-lookup"><span data-stu-id="ae7f2-135">groupId</span></span>|<span data-ttu-id="ae7f2-136">Guid</span><span class="sxs-lookup"><span data-stu-id="ae7f2-136">Guid</span></span>| <span data-ttu-id="ae7f2-137">Die Id der Gruppe erneuern.</span><span class="sxs-lookup"><span data-stu-id="ae7f2-137">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="ae7f2-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae7f2-138">Response</span></span>

<span data-ttu-id="ae7f2-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae7f2-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae7f2-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae7f2-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ae7f2-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae7f2-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "grouplifecyclepolicy_renewgroup"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/renewGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="ae7f2-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae7f2-143">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: renewgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->