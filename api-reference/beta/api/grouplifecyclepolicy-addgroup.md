---
title: 'groupLifecyclePolicy: addGroup'
description: Fügt eine Gruppe zu einer Lebenszyklusrichtlinie hinzu.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f5aee25421dea76b5bdb10f141d4e640c2196b94
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515510"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="32342-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="32342-103">groupLifecyclePolicy: addGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32342-104">Fügt eine Gruppe zu einer Lebenszyklusrichtlinie hinzu.</span><span class="sxs-lookup"><span data-stu-id="32342-104">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="32342-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="32342-105">Permissions</span></span>

<span data-ttu-id="32342-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32342-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="32342-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="32342-108">Permission type</span></span>      | <span data-ttu-id="32342-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="32342-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32342-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="32342-110">Delegated (work or school account)</span></span> | <span data-ttu-id="32342-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32342-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="32342-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="32342-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32342-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32342-113">Not supported</span></span> |
|<span data-ttu-id="32342-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="32342-114">Application</span></span> | <span data-ttu-id="32342-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32342-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="32342-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="32342-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="32342-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="32342-117">Request headers</span></span>

| <span data-ttu-id="32342-118">Name</span><span class="sxs-lookup"><span data-stu-id="32342-118">Name</span></span> | <span data-ttu-id="32342-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32342-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="32342-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="32342-120">Authorization</span></span> | <span data-ttu-id="32342-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="32342-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="32342-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32342-123">Content-Type</span></span>  | <span data-ttu-id="32342-124">application/json</span><span class="sxs-lookup"><span data-stu-id="32342-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="32342-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="32342-125">Request body</span></span>
<span data-ttu-id="32342-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="32342-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="32342-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="32342-127">Parameter</span></span> | <span data-ttu-id="32342-128">Typ</span><span class="sxs-lookup"><span data-stu-id="32342-128">Type</span></span> | <span data-ttu-id="32342-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32342-129">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="32342-130">groupId</span><span class="sxs-lookup"><span data-stu-id="32342-130">groupId</span></span>|<span data-ttu-id="32342-131">Guid</span><span class="sxs-lookup"><span data-stu-id="32342-131">Guid</span></span>| <span data-ttu-id="32342-132">Die ID der Gruppe, der die Richtlinie hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="32342-132">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="32342-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="32342-133">Response</span></span>

<span data-ttu-id="32342-134">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32342-134">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="32342-135">Wenn die Gruppe zur Richtlinie hinzugefügt wird, wird der Wert **true** im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32342-135">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="32342-136">Andernfalls wird der Wert **false** im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32342-136">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="32342-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="32342-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="32342-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="32342-138">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}/addGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

#### <a name="response"></a><span data-ttu-id="32342-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="32342-139">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "value": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-addgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
