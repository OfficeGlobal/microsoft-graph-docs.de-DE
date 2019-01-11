---
title: 'groupLifecyclePolicy: addGroup'
description: Fügt eine Gruppe zu einer Lebenszyklusrichtlinie hinzu.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: ac0bf455ba2d4aa5f1f6add5827124581ce663b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853361"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="b9bfa-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="b9bfa-103">groupLifecyclePolicy: addGroup</span></span>

> <span data-ttu-id="b9bfa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b9bfa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9bfa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9bfa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9bfa-106">Fügt eine Gruppe zu einer Lebenszyklusrichtlinie hinzu.</span><span class="sxs-lookup"><span data-stu-id="b9bfa-106">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9bfa-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b9bfa-107">Permissions</span></span>

<span data-ttu-id="b9bfa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9bfa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b9bfa-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9bfa-110">Permission type</span></span>      | <span data-ttu-id="b9bfa-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9bfa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9bfa-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9bfa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b9bfa-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9bfa-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="b9bfa-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9bfa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9bfa-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9bfa-115">Not supported</span></span> |
|<span data-ttu-id="b9bfa-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9bfa-116">Application</span></span> | <span data-ttu-id="b9bfa-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9bfa-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9bfa-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9bfa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="b9bfa-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9bfa-119">Request headers</span></span>

| <span data-ttu-id="b9bfa-120">Name</span><span class="sxs-lookup"><span data-stu-id="b9bfa-120">Name</span></span> | <span data-ttu-id="b9bfa-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9bfa-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b9bfa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9bfa-122">Authorization</span></span> | <span data-ttu-id="b9bfa-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b9bfa-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9bfa-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9bfa-125">Content-Type</span></span>  | <span data-ttu-id="b9bfa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9bfa-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9bfa-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9bfa-127">Request body</span></span>
<span data-ttu-id="b9bfa-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="b9bfa-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b9bfa-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="b9bfa-129">Parameter</span></span> | <span data-ttu-id="b9bfa-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b9bfa-130">Type</span></span> | <span data-ttu-id="b9bfa-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9bfa-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b9bfa-132">groupId</span><span class="sxs-lookup"><span data-stu-id="b9bfa-132">groupId</span></span>|<span data-ttu-id="b9bfa-133">Guid</span><span class="sxs-lookup"><span data-stu-id="b9bfa-133">Guid</span></span>| <span data-ttu-id="b9bfa-134">Die ID der Gruppe, der die Richtlinie hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b9bfa-134">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="b9bfa-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9bfa-135">Response</span></span>

<span data-ttu-id="b9bfa-136">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9bfa-136">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="b9bfa-137">Wenn die Gruppe zur Richtlinie hinzugefügt wird, wird der Wert **true** im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9bfa-137">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="b9bfa-138">Andernfalls wird der Wert **false** im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9bfa-138">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="b9bfa-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9bfa-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b9bfa-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9bfa-140">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b9bfa-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9bfa-141">Response</span></span>
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
