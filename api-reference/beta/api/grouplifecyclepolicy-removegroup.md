---
title: 'groupLifecyclePolicy: removeGroup'
description: Entfernt eine Gruppe aus einer Lebenszyklusrichtlinie.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3abf83c19132d0a8fe825c3e187a34dcc7114097
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915753"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="d8794-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="d8794-103">groupLifecyclePolicy: removeGroup</span></span>

> <span data-ttu-id="d8794-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d8794-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8794-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d8794-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d8794-106">Entfernt eine Gruppe aus einer Lebenszyklusrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="d8794-106">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8794-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d8794-107">Permissions</span></span>

<span data-ttu-id="d8794-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8794-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d8794-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d8794-110">Permission type</span></span>      | <span data-ttu-id="d8794-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d8794-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8794-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d8794-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d8794-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8794-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="d8794-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d8794-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8794-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d8794-115">Not supported</span></span> |
|<span data-ttu-id="d8794-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d8794-116">Application</span></span> |  <span data-ttu-id="d8794-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8794-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8794-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d8794-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="d8794-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d8794-119">Request headers</span></span>

| <span data-ttu-id="d8794-120">Name</span><span class="sxs-lookup"><span data-stu-id="d8794-120">Name</span></span> | <span data-ttu-id="d8794-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d8794-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d8794-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8794-122">Authorization</span></span> | <span data-ttu-id="d8794-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d8794-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d8794-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8794-125">Content-Type</span></span>  | <span data-ttu-id="d8794-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8794-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8794-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d8794-127">Request body</span></span>
<span data-ttu-id="d8794-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="d8794-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d8794-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="d8794-129">Parameter</span></span> | <span data-ttu-id="d8794-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d8794-130">Type</span></span> | <span data-ttu-id="d8794-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d8794-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d8794-132">groupId</span><span class="sxs-lookup"><span data-stu-id="d8794-132">groupId</span></span>|<span data-ttu-id="d8794-133">Guid</span><span class="sxs-lookup"><span data-stu-id="d8794-133">Guid</span></span>| <span data-ttu-id="d8794-134">Die ID der Gruppe, die aus der Richtlinie entfernt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d8794-134">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="d8794-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="d8794-135">Response</span></span>

<span data-ttu-id="d8794-136">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d8794-136">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="d8794-137">Wenn die Gruppe aus der Richtlinie entfernt wird, wird der Wert **true** im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d8794-137">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="d8794-138">Andernfalls wird der Wert **false** im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d8794-138">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="d8794-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d8794-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d8794-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d8794-140">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="d8794-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="d8794-141">Response</span></span>
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
