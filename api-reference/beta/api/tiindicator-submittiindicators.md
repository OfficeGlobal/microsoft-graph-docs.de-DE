---
title: 'tiIndicator: submitTiIndicators'
description: Laden Sie mehrere Threat Intelligence-Indikatoren (TI) in einer Anforderung anstelle mehrerer Anforderungen hoch.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: b6d3e530fc571029c3b71675ca195e7bb046c823
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366973"
---
# <a name="tiindicator-submittiindicators"></a><span data-ttu-id="cef30-103">tiIndicator: submitTiIndicators</span><span class="sxs-lookup"><span data-stu-id="cef30-103">tiIndicator: submitTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cef30-104">Laden Sie mehrere Threat Intelligence-Indikatoren (TI) in einer Anforderung anstelle mehrerer Anforderungen hoch.</span><span class="sxs-lookup"><span data-stu-id="cef30-104">Upload multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="cef30-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cef30-105">Permissions</span></span>

<span data-ttu-id="cef30-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cef30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cef30-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cef30-108">Permission type</span></span> | <span data-ttu-id="cef30-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cef30-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cef30-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cef30-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cef30-111">ThreatIndicators. ReadWrite. OwnedBy</span><span class="sxs-lookup"><span data-stu-id="cef30-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="cef30-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cef30-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cef30-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cef30-113">Not supported.</span></span> |
| <span data-ttu-id="cef30-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cef30-114">Application</span></span>                            | <span data-ttu-id="cef30-115">ThreatIndicators. ReadWrite. OwnedBy</span><span class="sxs-lookup"><span data-stu-id="cef30-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="cef30-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cef30-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/submitTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="cef30-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cef30-117">Request headers</span></span>

| <span data-ttu-id="cef30-118">Name</span><span class="sxs-lookup"><span data-stu-id="cef30-118">Name</span></span>          | <span data-ttu-id="cef30-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cef30-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cef30-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cef30-120">Authorization</span></span> | <span data-ttu-id="cef30-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="cef30-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="cef30-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cef30-122">Request body</span></span>

<span data-ttu-id="cef30-123">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="cef30-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cef30-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="cef30-124">Parameter</span></span>    | <span data-ttu-id="cef30-125">Typ</span><span class="sxs-lookup"><span data-stu-id="cef30-125">Type</span></span>        | <span data-ttu-id="cef30-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cef30-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cef30-127">Wert</span><span class="sxs-lookup"><span data-stu-id="cef30-127">value</span></span>|<span data-ttu-id="cef30-128">tiIndicator-Sammlung</span><span class="sxs-lookup"><span data-stu-id="cef30-128">tiIndicator collection</span></span>| <span data-ttu-id="cef30-129">JSON-Auflistung von **tiIndicators** , die erstellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="cef30-129">JSON collection of **tiIndicators** to be created.</span></span> |

## <a name="response"></a><span data-ttu-id="cef30-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="cef30-130">Response</span></span>

<span data-ttu-id="cef30-131">Bei erfolgreicher Ausführung gibt diese Methode `200, OK` den Antwortcode und ein [tiIndicator](../resources/tiindicator.md) -Auflistungsobjekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cef30-131">If successful, this method returns `200, OK` response code and a [tiIndicator](../resources/tiindicator.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cef30-132">Beispiele</span><span class="sxs-lookup"><span data-stu-id="cef30-132">Examples</span></span>

<span data-ttu-id="cef30-133">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="cef30-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="cef30-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cef30-134">Request</span></span>

<span data-ttu-id="cef30-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cef30-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tiindicator_submittiindicators"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/submitTiIndicators
Content-type: application/json

{
  "value": [
    {
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
      "expirationDateTime": "2019-03-01T21:44:03.1668987+00:00",
      "externalId": "Test--8586509942423126760MS164-0",
      "fileHashType": "sha256",
      "fileHashValue": "b555c45c5b1b01304217e72118d6ca1b14b7013644a078273cea27bbdc1cf9d6",
      "killChain": [],
      "malwareFamilyNames": [],
      "severity": 0,
      "tags": [],
      "targetProduct": "Azure Sentinel",
      "threatType": "WatchList",
      "tlpLevel": "green",
    },
    {
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
      "expirationDateTime": "2019-03-01T21:44:03.1748779+00:00",
      "externalId": "Test--8586509942423126760MS164-1",
      "fileHashType": "sha256",
      "fileHashValue": "1796b433950990b28d6a22456c9d2b58ced1bdfcdf5f16f7e39d6b9bdca4213b",
      "killChain": [],
      "malwareFamilyNames": [],
      "severity": 0,
      "tags": [],
      "targetProduct": "Azure Sentinel",
      "threatType": "WatchList",
      "tlpLevel": "green",
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="cef30-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="cef30-136">Response</span></span>

<span data-ttu-id="cef30-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cef30-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="cef30-138">Das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="cef30-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cef30-139">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="cef30-139">All the properties will be returned from an actual call.</span></span>

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
      "azureTenantId": "XXXXXXXXXXXXXXXXXXXXX",
      "action": null,
      "additionalInformation": null,
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
  "description": "tiIndicator: submitTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->