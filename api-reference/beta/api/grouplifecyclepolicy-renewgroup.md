---
title: 'GroupLifecyclePolicy: RenewGroup'
description: Verlängert den Ablaufzeitraum einer Gruppe. Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 7eb0ef44a5e07c8c293ba804cc8ec31a8312576d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520872"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="09075-104">GroupLifecyclePolicy: RenewGroup</span><span class="sxs-lookup"><span data-stu-id="09075-104">groupLifecyclePolicy: renewGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09075-105">Verlängert den Ablaufzeitraum einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="09075-105">Renews a group's expiration.</span></span> <span data-ttu-id="09075-106">Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind.</span><span class="sxs-lookup"><span data-stu-id="09075-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="09075-107">**Hinweis:** In v1. 0, [Verwenden Sie die Gruppenressource um Anfragen erneuern zu machen](/graph/api/group-renew?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="09075-107">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="09075-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="09075-108">Permissions</span></span>

<span data-ttu-id="09075-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09075-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="09075-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="09075-111">Permission type</span></span>      | <span data-ttu-id="09075-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="09075-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09075-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="09075-113">Delegated (work or school account)</span></span> | <span data-ttu-id="09075-114">Group.ReadWrite.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09075-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="09075-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="09075-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09075-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09075-116">Not supported</span></span> |
|<span data-ttu-id="09075-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="09075-117">Application</span></span> | <span data-ttu-id="09075-118">Group.ReadWrite.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09075-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09075-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="09075-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="09075-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="09075-120">Request headers</span></span>

| <span data-ttu-id="09075-121">Name</span><span class="sxs-lookup"><span data-stu-id="09075-121">Name</span></span> | <span data-ttu-id="09075-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09075-122">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="09075-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="09075-123">Authorization</span></span> | <span data-ttu-id="09075-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="09075-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="09075-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="09075-126">Content-Type</span></span>  | <span data-ttu-id="09075-127">application/json</span><span class="sxs-lookup"><span data-stu-id="09075-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="09075-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="09075-128">Request body</span></span>
<span data-ttu-id="09075-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="09075-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="09075-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="09075-130">Parameter</span></span> | <span data-ttu-id="09075-131">Typ</span><span class="sxs-lookup"><span data-stu-id="09075-131">Type</span></span> | <span data-ttu-id="09075-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09075-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="09075-133">groupId</span><span class="sxs-lookup"><span data-stu-id="09075-133">groupId</span></span>|<span data-ttu-id="09075-134">Guid</span><span class="sxs-lookup"><span data-stu-id="09075-134">Guid</span></span>| <span data-ttu-id="09075-135">Die Id der Gruppe erneuern.</span><span class="sxs-lookup"><span data-stu-id="09075-135">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="09075-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="09075-136">Response</span></span>

<span data-ttu-id="09075-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="09075-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09075-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="09075-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="09075-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="09075-140">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="09075-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="09075-141">Response</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: renewgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-renewgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
