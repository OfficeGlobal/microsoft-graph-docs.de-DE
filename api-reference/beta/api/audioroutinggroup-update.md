---
title: Audio Routinggruppe aktualisieren
description: Inhaltsquellen und der Empfänger von einer AudioRoutingGroup zu ändern.
author: VinodRavichandran
ms.openlocfilehash: ae9e67a9f116a9c1e9dec2b5d742f13917374718
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336687"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="247b1-103">Audio Routinggruppe aktualisieren</span><span class="sxs-lookup"><span data-stu-id="247b1-103">Update audio routing group</span></span>

> <span data-ttu-id="247b1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="247b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="247b1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="247b1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="247b1-106">Inhaltsquellen und der Empfänger von einer [AudioRoutingGroup](../resources/audioroutinggroup.md)zu ändern.</span><span class="sxs-lookup"><span data-stu-id="247b1-106">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="247b1-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="247b1-107">Permissions</span></span>
<span data-ttu-id="247b1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="247b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="247b1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="247b1-110">Permission type</span></span> | <span data-ttu-id="247b1-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="247b1-111">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="247b1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="247b1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="247b1-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="247b1-113">Not Supported</span></span>                       |
| <span data-ttu-id="247b1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="247b1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="247b1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="247b1-115">Not Supported</span></span>                       |
| <span data-ttu-id="247b1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="247b1-116">Application</span></span>     | <span data-ttu-id="247b1-117">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="247b1-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="247b1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="247b1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="247b1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="247b1-119">Request headers</span></span>
| <span data-ttu-id="247b1-120">Name</span><span class="sxs-lookup"><span data-stu-id="247b1-120">Name</span></span>          | <span data-ttu-id="247b1-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="247b1-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="247b1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="247b1-122">Authorization</span></span> | <span data-ttu-id="247b1-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="247b1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="247b1-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="247b1-125">Request body</span></span>
<span data-ttu-id="247b1-126">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="247b1-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="247b1-127">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="247b1-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="247b1-128">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="247b1-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="247b1-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="247b1-129">Property</span></span>       | <span data-ttu-id="247b1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="247b1-130">Type</span></span>    |<span data-ttu-id="247b1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="247b1-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="247b1-132">Ereignisempfänger</span><span class="sxs-lookup"><span data-stu-id="247b1-132">receivers</span></span> | <span data-ttu-id="247b1-133">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="247b1-133">String collection</span></span> | <span data-ttu-id="247b1-134">Die Ziel-Teilnehmer in der AudioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="247b1-134">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="247b1-135">routingMode</span><span class="sxs-lookup"><span data-stu-id="247b1-135">routingMode</span></span> | <span data-ttu-id="247b1-136">String</span><span class="sxs-lookup"><span data-stu-id="247b1-136">String</span></span> | <span data-ttu-id="247b1-137">Mögliche Werte: `oneToOne`, `multicast`.</span><span class="sxs-lookup"><span data-stu-id="247b1-137">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="247b1-138">sources</span><span class="sxs-lookup"><span data-stu-id="247b1-138">sources</span></span> | <span data-ttu-id="247b1-139">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="247b1-139">String collection</span></span> | <span data-ttu-id="247b1-140">Die Quelle Teilnehmer in der AudioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="247b1-140">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="247b1-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="247b1-141">Response</span></span>
<span data-ttu-id="247b1-142">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AudioRoutingGroup](../resources/audioroutinggroup.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="247b1-142">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="247b1-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="247b1-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="247b1-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="247b1-144">Request</span></span>
<span data-ttu-id="247b1-145">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="247b1-145">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_audioRoutingGroup"
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
##### <a name="response"></a><span data-ttu-id="247b1-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="247b1-146">Response</span></span>

> <span data-ttu-id="247b1-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="247b1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
