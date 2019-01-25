---
title: Erstellen von audio Routinggruppe
description: Erstellen Sie eine neue **AudioRoutingGroup**.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: dc0e2a3463229762b3a641f33f77f2df8d506aa0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522861"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="1f22c-103">Erstellen von audio Routinggruppe</span><span class="sxs-lookup"><span data-stu-id="1f22c-103">Create audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f22c-104">Erstellen Sie eine neue **AudioRoutingGroup**.</span><span class="sxs-lookup"><span data-stu-id="1f22c-104">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f22c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1f22c-105">Permissions</span></span>
<span data-ttu-id="1f22c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f22c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1f22c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1f22c-108">Permission type</span></span>                        | <span data-ttu-id="1f22c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1f22c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1f22c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1f22c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f22c-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f22c-111">Not supported.</span></span>                               |
| <span data-ttu-id="1f22c-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1f22c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f22c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f22c-113">Not supported.</span></span>                               |
| <span data-ttu-id="1f22c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1f22c-114">Application</span></span>                            | <span data-ttu-id="1f22c-115">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="1f22c-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f22c-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f22c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="request-headers"></a><span data-ttu-id="1f22c-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1f22c-117">Request headers</span></span>
| <span data-ttu-id="1f22c-118">Name</span><span class="sxs-lookup"><span data-stu-id="1f22c-118">Name</span></span>          | <span data-ttu-id="1f22c-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f22c-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1f22c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f22c-120">Authorization</span></span> | <span data-ttu-id="1f22c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1f22c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f22c-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1f22c-123">Request body</span></span>
<span data-ttu-id="1f22c-124">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [AudioRoutingGroup](../resources/audioroutinggroup.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1f22c-124">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1f22c-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f22c-125">Response</span></span>
<span data-ttu-id="1f22c-126">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekt Code und [AudioRoutingGroup](../resources/audioroutinggroup.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1f22c-126">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f22c-127">Beispiele</span><span class="sxs-lookup"><span data-stu-id="1f22c-127">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="1f22c-128">In Beispiel 1: 1: 1-audio Routinggruppe</span><span class="sxs-lookup"><span data-stu-id="1f22c-128">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="1f22c-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f22c-129">Request</span></span>
<span data-ttu-id="1f22c-130">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="1f22c-130">The following example shows the request.</span></span>

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

<span data-ttu-id="1f22c-131">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [AudioRoutingGroup](../resources/audioroutinggroup.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1f22c-131">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="1f22c-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f22c-132">Response</span></span>

> <span data-ttu-id="1f22c-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="1f22c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="1f22c-135">Beispiel 2: Multicast audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="1f22c-135">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="1f22c-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f22c-136">Request</span></span>
<span data-ttu-id="1f22c-137">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="1f22c-137">The following example shows the request.</span></span>

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

<span data-ttu-id="1f22c-138">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [AudioRoutingGroup](../resources/audioroutinggroup.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1f22c-138">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="1f22c-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f22c-139">Response</span></span>

> <span data-ttu-id="1f22c-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="1f22c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Create audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-post-audioroutinggroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
