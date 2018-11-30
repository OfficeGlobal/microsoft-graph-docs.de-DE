---
title: 'groupLifecyclePolicy: addGroup'
description: Fügt eine Gruppe zu einer Lebenszyklusrichtlinie hinzu.
ms.openlocfilehash: efcb7a29814049ba6e7c5d063c6744e5a3646b67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018142"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="6114d-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="6114d-103">groupLifecyclePolicy: addGroup</span></span>

<span data-ttu-id="6114d-104">Fügt eine Gruppe zu einer Lebenszyklusrichtlinie hinzu.</span><span class="sxs-lookup"><span data-stu-id="6114d-104">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="6114d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6114d-105">Permissions</span></span>

<span data-ttu-id="6114d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6114d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6114d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6114d-108">Permission type</span></span>      | <span data-ttu-id="6114d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6114d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6114d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6114d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6114d-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6114d-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="6114d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6114d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6114d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6114d-113">Not supported.</span></span>    |
|<span data-ttu-id="6114d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6114d-114">Application</span></span> | <span data-ttu-id="6114d-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6114d-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6114d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6114d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="6114d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6114d-117">Request headers</span></span>

| <span data-ttu-id="6114d-118">Name</span><span class="sxs-lookup"><span data-stu-id="6114d-118">Name</span></span> | <span data-ttu-id="6114d-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6114d-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="6114d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6114d-120">Authorization</span></span> | <span data-ttu-id="6114d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6114d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6114d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6114d-123">Content-Type</span></span>  | <span data-ttu-id="6114d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6114d-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6114d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6114d-125">Request body</span></span>
<span data-ttu-id="6114d-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="6114d-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6114d-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="6114d-127">Parameter</span></span> | <span data-ttu-id="6114d-128">Typ</span><span class="sxs-lookup"><span data-stu-id="6114d-128">Type</span></span> | <span data-ttu-id="6114d-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6114d-129">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6114d-130">groupId</span><span class="sxs-lookup"><span data-stu-id="6114d-130">groupId</span></span>|<span data-ttu-id="6114d-131">Guid</span><span class="sxs-lookup"><span data-stu-id="6114d-131">Guid</span></span>| <span data-ttu-id="6114d-132">Die ID der Gruppe, der die Richtlinie hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="6114d-132">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="6114d-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="6114d-133">Response</span></span>

<span data-ttu-id="6114d-134">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6114d-134">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="6114d-135">Wenn die Gruppe zur Richtlinie hinzugefügt wird, wird der Wert **true** im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6114d-135">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="6114d-136">Andernfalls wird der Wert **false** im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6114d-136">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="6114d-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6114d-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6114d-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6114d-138">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/addGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

#### <a name="response"></a><span data-ttu-id="6114d-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="6114d-139">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->