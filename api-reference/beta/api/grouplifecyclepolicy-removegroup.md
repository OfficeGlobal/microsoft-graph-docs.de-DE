---
title: 'groupLifecyclePolicy: removeGroup'
description: Entfernt eine Gruppe aus einer Lebenszyklusrichtlinie.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: faf394e411301d268a307151d98ec84a9b4e19a9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894127"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="cb8e2-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="cb8e2-103">groupLifecyclePolicy: removeGroup</span></span>

> <span data-ttu-id="cb8e2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cb8e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb8e2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cb8e2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cb8e2-106">Entfernt eine Gruppe aus einer Lebenszyklusrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="cb8e2-106">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb8e2-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cb8e2-107">Permissions</span></span>

<span data-ttu-id="cb8e2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb8e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cb8e2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cb8e2-110">Permission type</span></span>      | <span data-ttu-id="cb8e2-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cb8e2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb8e2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cb8e2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cb8e2-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb8e2-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="cb8e2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cb8e2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb8e2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cb8e2-115">Not supported</span></span> |
|<span data-ttu-id="cb8e2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cb8e2-116">Application</span></span> |  <span data-ttu-id="cb8e2-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb8e2-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb8e2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb8e2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="cb8e2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cb8e2-119">Request headers</span></span>

| <span data-ttu-id="cb8e2-120">Name</span><span class="sxs-lookup"><span data-stu-id="cb8e2-120">Name</span></span> | <span data-ttu-id="cb8e2-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb8e2-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="cb8e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb8e2-122">Authorization</span></span> | <span data-ttu-id="cb8e2-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cb8e2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cb8e2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb8e2-125">Content-Type</span></span>  | <span data-ttu-id="cb8e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb8e2-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb8e2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cb8e2-127">Request body</span></span>
<span data-ttu-id="cb8e2-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="cb8e2-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cb8e2-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="cb8e2-129">Parameter</span></span> | <span data-ttu-id="cb8e2-130">Typ</span><span class="sxs-lookup"><span data-stu-id="cb8e2-130">Type</span></span> | <span data-ttu-id="cb8e2-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb8e2-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cb8e2-132">groupId</span><span class="sxs-lookup"><span data-stu-id="cb8e2-132">groupId</span></span>|<span data-ttu-id="cb8e2-133">Guid</span><span class="sxs-lookup"><span data-stu-id="cb8e2-133">Guid</span></span>| <span data-ttu-id="cb8e2-134">Die ID der Gruppe, die aus der Richtlinie entfernt werden soll.</span><span class="sxs-lookup"><span data-stu-id="cb8e2-134">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="cb8e2-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb8e2-135">Response</span></span>

<span data-ttu-id="cb8e2-136">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb8e2-136">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="cb8e2-137">Wenn die Gruppe aus der Richtlinie entfernt wird, wird der Wert **true** im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb8e2-137">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="cb8e2-138">Andernfalls wird der Wert **false** im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb8e2-138">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="cb8e2-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cb8e2-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cb8e2-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb8e2-140">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_removegroup"
} -->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}/removeGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="cb8e2-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb8e2-141">Response</span></span>
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
  "description": "groupLifecyclePolicy: removegroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
