---
title: Erstellen von audio Routinggruppe
description: Erstellen Sie eine neue **AudioRoutingGroup**.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fe623a581233324e13c949d16570b1396fdd663c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966384"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="3bf81-103">Erstellen von audio Routinggruppe</span><span class="sxs-lookup"><span data-stu-id="3bf81-103">Create audio routing group</span></span>

> <span data-ttu-id="3bf81-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3bf81-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3bf81-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3bf81-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3bf81-106">Erstellen Sie eine neue **AudioRoutingGroup**.</span><span class="sxs-lookup"><span data-stu-id="3bf81-106">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="3bf81-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3bf81-107">Permissions</span></span>
<span data-ttu-id="3bf81-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bf81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3bf81-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3bf81-110">Permission type</span></span>                        | <span data-ttu-id="3bf81-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3bf81-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3bf81-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3bf81-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3bf81-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3bf81-113">Not supported.</span></span>                               |
| <span data-ttu-id="3bf81-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3bf81-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bf81-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3bf81-115">Not supported.</span></span>                               |
| <span data-ttu-id="3bf81-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3bf81-116">Application</span></span>                            | <span data-ttu-id="3bf81-117">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="3bf81-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bf81-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3bf81-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="request-headers"></a><span data-ttu-id="3bf81-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3bf81-119">Request headers</span></span>
| <span data-ttu-id="3bf81-120">Name</span><span class="sxs-lookup"><span data-stu-id="3bf81-120">Name</span></span>          | <span data-ttu-id="3bf81-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3bf81-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3bf81-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bf81-122">Authorization</span></span> | <span data-ttu-id="3bf81-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3bf81-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3bf81-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3bf81-125">Request body</span></span>
<span data-ttu-id="3bf81-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [AudioRoutingGroup](../resources/audioroutinggroup.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3bf81-126">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3bf81-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="3bf81-127">Response</span></span>
<span data-ttu-id="3bf81-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekt Code und [AudioRoutingGroup](../resources/audioroutinggroup.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3bf81-128">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3bf81-129">Beispiele</span><span class="sxs-lookup"><span data-stu-id="3bf81-129">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="3bf81-130">In Beispiel 1: 1: 1-audio Routinggruppe</span><span class="sxs-lookup"><span data-stu-id="3bf81-130">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="3bf81-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3bf81-131">Request</span></span>
<span data-ttu-id="3bf81-132">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="3bf81-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-audioRoutingGroup-from-call"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f"
  ]
}
```

<span data-ttu-id="3bf81-133">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [AudioRoutingGroup](../resources/audioroutinggroup.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3bf81-133">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="3bf81-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3bf81-134">Response</span></span>

> <span data-ttu-id="3bf81-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="3bf81-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f"
  ]
}
```
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="3bf81-137">Beispiel 2: Multicast audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="3bf81-137">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="3bf81-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3bf81-138">Request</span></span>
<span data-ttu-id="3bf81-139">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="3bf81-139">The following example shows the request.</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
Content-Type: application/json
Content-Length: 233
```

<!-- {
  "blockType": "example",
  "name": "create-audioRoutingGroup-from-call",
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->

```json
{
  "id": "multicast",
  "routingMode": "multicast",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```

<span data-ttu-id="3bf81-140">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [AudioRoutingGroup](../resources/audioroutinggroup.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3bf81-140">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="3bf81-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="3bf81-141">Response</span></span>

> <span data-ttu-id="3bf81-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="3bf81-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233
```
<!-- {
  "blockType": "example",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->

```json
{
  "id": "multicast",
  "routingMode": "multicast",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
