---
title: 'GroupLifecyclePolicy: RenewGroup'
description: Verlängert den Ablaufzeitraum einer Gruppe. Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 8facbd22887e99fc3b7edcdcb17940d0845cd31d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960406"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="97548-104">GroupLifecyclePolicy: RenewGroup</span><span class="sxs-lookup"><span data-stu-id="97548-104">groupLifecyclePolicy: renewGroup</span></span>

> <span data-ttu-id="97548-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="97548-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97548-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="97548-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97548-107">Verlängert den Ablaufzeitraum einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="97548-107">Renews a group's expiration.</span></span> <span data-ttu-id="97548-108">Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind.</span><span class="sxs-lookup"><span data-stu-id="97548-108">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="97548-109">**Hinweis:** In v1. 0, [Verwenden Sie die Gruppenressource um Anfragen erneuern zu machen](/graph/api/group-renew?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="97548-109">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="97548-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="97548-110">Permissions</span></span>

<span data-ttu-id="97548-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97548-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="97548-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97548-113">Permission type</span></span>      | <span data-ttu-id="97548-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97548-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97548-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97548-115">Delegated (work or school account)</span></span> | <span data-ttu-id="97548-116">Group.ReadWrite.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97548-116">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="97548-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97548-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97548-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97548-118">Not supported</span></span> |
|<span data-ttu-id="97548-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97548-119">Application</span></span> | <span data-ttu-id="97548-120">Group.ReadWrite.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97548-120">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97548-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97548-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="97548-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97548-122">Request headers</span></span>

| <span data-ttu-id="97548-123">Name</span><span class="sxs-lookup"><span data-stu-id="97548-123">Name</span></span> | <span data-ttu-id="97548-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97548-124">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="97548-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="97548-125">Authorization</span></span> | <span data-ttu-id="97548-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="97548-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="97548-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97548-128">Content-Type</span></span>  | <span data-ttu-id="97548-129">application/json</span><span class="sxs-lookup"><span data-stu-id="97548-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="97548-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97548-130">Request body</span></span>
<span data-ttu-id="97548-131">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="97548-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="97548-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="97548-132">Parameter</span></span> | <span data-ttu-id="97548-133">Typ</span><span class="sxs-lookup"><span data-stu-id="97548-133">Type</span></span> | <span data-ttu-id="97548-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97548-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="97548-135">groupId</span><span class="sxs-lookup"><span data-stu-id="97548-135">groupId</span></span>|<span data-ttu-id="97548-136">Guid</span><span class="sxs-lookup"><span data-stu-id="97548-136">Guid</span></span>| <span data-ttu-id="97548-137">Die Id der Gruppe erneuern.</span><span class="sxs-lookup"><span data-stu-id="97548-137">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="97548-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="97548-138">Response</span></span>

<span data-ttu-id="97548-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97548-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97548-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97548-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="97548-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97548-142">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="97548-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="97548-143">Response</span></span>

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
