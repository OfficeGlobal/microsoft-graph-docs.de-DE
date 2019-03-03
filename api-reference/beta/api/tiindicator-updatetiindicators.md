---
title: 'tiIndicator: updateTiIndicators'
description: Aktualisieren Sie mehrere Threat Intelligence-Indikatoren (TI) in einer Anforderung anstelle mehrerer Anforderungen.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 91020b533b621c1ba77b2f839d4e6ffd8d7ee8ac
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30367141"
---
# <a name="tiindicator-updatetiindicators"></a><span data-ttu-id="2b1db-103">tiIndicator: updateTiIndicators</span><span class="sxs-lookup"><span data-stu-id="2b1db-103">tiIndicator: updateTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b1db-104">Aktualisieren Sie mehrere Threat Intelligence-Indikatoren (TI) in einer Anforderung anstelle mehrerer Anforderungen.</span><span class="sxs-lookup"><span data-stu-id="2b1db-104">Update multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b1db-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2b1db-105">Permissions</span></span>

<span data-ttu-id="2b1db-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b1db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2b1db-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2b1db-108">Permission type</span></span>   | <span data-ttu-id="2b1db-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2b1db-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2b1db-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2b1db-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2b1db-111">ThreatIndicators. ReadWrite. OwnedBy</span><span class="sxs-lookup"><span data-stu-id="2b1db-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="2b1db-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2b1db-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b1db-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b1db-113">Not supported.</span></span> |
| <span data-ttu-id="2b1db-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2b1db-114">Application</span></span>                            | <span data-ttu-id="2b1db-115">ThreatIndicators. ReadWrite. OwnedBy</span><span class="sxs-lookup"><span data-stu-id="2b1db-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b1db-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b1db-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/updateTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="2b1db-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2b1db-117">Request headers</span></span>

| <span data-ttu-id="2b1db-118">Name</span><span class="sxs-lookup"><span data-stu-id="2b1db-118">Name</span></span>          | <span data-ttu-id="2b1db-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b1db-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2b1db-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b1db-120">Authorization</span></span> | <span data-ttu-id="2b1db-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2b1db-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b1db-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2b1db-122">Request body</span></span>

<span data-ttu-id="2b1db-123">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="2b1db-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="2b1db-124">Ausführliche Informationen zu Eigenschaften, die aktualisiert werden können, finden Sie unter [Update tiIndicator](tiindicator-update.md).</span><span class="sxs-lookup"><span data-stu-id="2b1db-124">For details about properties that can be updated, see [update tiIndicator](tiindicator-update.md).</span></span>

| <span data-ttu-id="2b1db-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="2b1db-125">Parameter</span></span>    | <span data-ttu-id="2b1db-126">Typ</span><span class="sxs-lookup"><span data-stu-id="2b1db-126">Type</span></span>        | <span data-ttu-id="2b1db-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b1db-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2b1db-128">Wert</span><span class="sxs-lookup"><span data-stu-id="2b1db-128">value</span></span>|<span data-ttu-id="2b1db-129">tiIndicator-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2b1db-129">tiIndicator collection</span></span>| <span data-ttu-id="2b1db-130">Sammlung von **tiIndicators** , die aktualisiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="2b1db-130">Collection of **tiIndicators** to update.</span></span> <span data-ttu-id="2b1db-131">Jede Entität muss **ID** und andere bearbeitbare Eigenschaften haben, die aktualisiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="2b1db-131">Each entity must have **id** and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="2b1db-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b1db-132">Response</span></span>

<span data-ttu-id="2b1db-133">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [tiIndicator](../resources/tiindicator.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2b1db-133">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2b1db-134">Beispiele</span><span class="sxs-lookup"><span data-stu-id="2b1db-134">Examples</span></span>

<span data-ttu-id="2b1db-135">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="2b1db-135">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="2b1db-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b1db-136">Request</span></span>

<span data-ttu-id="2b1db-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2b1db-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tiindicator_updatetiindicators"
}-->
```http
POST https://graph.microsoft.com/beta/security/tiIndicators/updateTiIndicators
Content-type: application/json

{
  "value": [
    {
      "id": "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
      "additionalInformation": "mytest"
    },
    {
      "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
      "additionalInformation": "test again"
    }
  ]
}

```

### <a name="response"></a><span data-ttu-id="2b1db-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b1db-138">Response</span></span>

<span data-ttu-id="2b1db-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2b1db-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="2b1db-140">Das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="2b1db-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2b1db-141">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="2b1db-141">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.tiIndicator",
      "id": "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
      "azureTenantId": "XXXXXXXXXXXXXXXXXX",
      "action": null,
      "additionalInformation": "mytest",
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a test indicator for demo purpose. Take no action on any observables set in this indicator.",
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: updateTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
