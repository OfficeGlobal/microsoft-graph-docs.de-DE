---
title: Audio Routinggruppe aktualisieren
description: Inhaltsquellen und der Empfänger von einer AudioRoutingGroup zu ändern.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 02a6c8142ec36becd2a06a16d81bff7d1ceff75b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524674"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="454a1-103">Audio Routinggruppe aktualisieren</span><span class="sxs-lookup"><span data-stu-id="454a1-103">Update audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="454a1-104">Inhaltsquellen und der Empfänger von einer [AudioRoutingGroup](../resources/audioroutinggroup.md)zu ändern.</span><span class="sxs-lookup"><span data-stu-id="454a1-104">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="454a1-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="454a1-105">Permissions</span></span>
<span data-ttu-id="454a1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="454a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="454a1-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="454a1-108">Permission type</span></span> | <span data-ttu-id="454a1-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="454a1-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="454a1-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="454a1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="454a1-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="454a1-111">Not Supported</span></span>                       |
| <span data-ttu-id="454a1-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="454a1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="454a1-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="454a1-113">Not Supported</span></span>                       |
| <span data-ttu-id="454a1-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="454a1-114">Application</span></span>     | <span data-ttu-id="454a1-115">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="454a1-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="454a1-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="454a1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="454a1-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="454a1-117">Request headers</span></span>
| <span data-ttu-id="454a1-118">Name</span><span class="sxs-lookup"><span data-stu-id="454a1-118">Name</span></span>          | <span data-ttu-id="454a1-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="454a1-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="454a1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="454a1-120">Authorization</span></span> | <span data-ttu-id="454a1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="454a1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="454a1-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="454a1-123">Request body</span></span>
<span data-ttu-id="454a1-124">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="454a1-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="454a1-125">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="454a1-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="454a1-126">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="454a1-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="454a1-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="454a1-127">Property</span></span>       | <span data-ttu-id="454a1-128">Typ</span><span class="sxs-lookup"><span data-stu-id="454a1-128">Type</span></span>    |<span data-ttu-id="454a1-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="454a1-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="454a1-130">Ereignisempfänger</span><span class="sxs-lookup"><span data-stu-id="454a1-130">receivers</span></span> | <span data-ttu-id="454a1-131">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="454a1-131">String collection</span></span> | <span data-ttu-id="454a1-132">Die Ziel-Teilnehmer in der AudioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="454a1-132">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="454a1-133">routingMode</span><span class="sxs-lookup"><span data-stu-id="454a1-133">routingMode</span></span> | <span data-ttu-id="454a1-134">String</span><span class="sxs-lookup"><span data-stu-id="454a1-134">String</span></span> | <span data-ttu-id="454a1-135">Mögliche Werte: `oneToOne`, `multicast`.</span><span class="sxs-lookup"><span data-stu-id="454a1-135">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="454a1-136">sources</span><span class="sxs-lookup"><span data-stu-id="454a1-136">sources</span></span> | <span data-ttu-id="454a1-137">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="454a1-137">String collection</span></span> | <span data-ttu-id="454a1-138">Die Quelle Teilnehmer in der AudioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="454a1-138">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="454a1-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="454a1-139">Response</span></span>
<span data-ttu-id="454a1-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AudioRoutingGroup](../resources/audioroutinggroup.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="454a1-140">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="454a1-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="454a1-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="454a1-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="454a1-142">Request</span></span>
<span data-ttu-id="454a1-143">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="454a1-143">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update-audioRoutingGroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```
##### <a name="response"></a><span data-ttu-id="454a1-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="454a1-144">Response</span></span>

> <span data-ttu-id="454a1-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="454a1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Update audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/audioroutinggroup-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
