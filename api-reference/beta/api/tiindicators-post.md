---
title: Bedrohungs Intelligenz-Indikator erstellen
description: Erstellen Sie eine neue tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 440515a45b4c530f32dd20fe29497e338b54a6bf
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481440"
---
# <a name="create-threat-intelligence-indicator"></a><span data-ttu-id="7ba34-103">Bedrohungs Intelligenz-Indikator erstellen</span><span class="sxs-lookup"><span data-stu-id="7ba34-103">Create threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ba34-104">Erstellen eines neuen [tiIndicator](../resources/tiindicator.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7ba34-104">Create a new [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ba34-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7ba34-105">Permissions</span></span>

<span data-ttu-id="7ba34-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ba34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7ba34-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7ba34-108">Permission type</span></span>                        | <span data-ttu-id="7ba34-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7ba34-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7ba34-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7ba34-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ba34-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="7ba34-111">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="7ba34-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7ba34-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ba34-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ba34-113">Not supported.</span></span> |
| <span data-ttu-id="7ba34-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7ba34-114">Application</span></span>                            | <span data-ttu-id="7ba34-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="7ba34-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ba34-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ba34-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="7ba34-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7ba34-117">Request headers</span></span>

| <span data-ttu-id="7ba34-118">Name</span><span class="sxs-lookup"><span data-stu-id="7ba34-118">Name</span></span>          | <span data-ttu-id="7ba34-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ba34-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7ba34-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ba34-120">Authorization</span></span> | <span data-ttu-id="7ba34-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7ba34-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ba34-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7ba34-122">Request body</span></span>

<span data-ttu-id="7ba34-123">Geben Sie im Anforderungstext eine JSON-Darstellung eines [tiIndicator](../resources/tiindicator.md) -Objekts an, das mindestens eine zu beobachtbare [e-Mail](../resources/tiindicator.md#indicator-observables---email), [Datei](../resources/tiindicator.md#indicator-observables---file)oder ein [Netzwerk](../resources/tiindicator.md#indicator-observables---network) enthält.</span><span class="sxs-lookup"><span data-stu-id="7ba34-123">In the request body, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable.</span></span>

## <a name="response"></a><span data-ttu-id="7ba34-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ba34-124">Response</span></span>

<span data-ttu-id="7ba34-125">Bei erfolgreicher Ausführung gibt diese Methode `201 Created` den Antwortcode und ein [tiIndicator](../resources/tiindicator.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7ba34-125">If successful, this method returns `201 Created` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7ba34-126">Beispiele</span><span class="sxs-lookup"><span data-stu-id="7ba34-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7ba34-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ba34-127">Request</span></span>

<span data-ttu-id="7ba34-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7ba34-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tiindicator_from_security"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators
Content-type: application/json

{
  "action": "alert",
  "activityGroupNames": [],
  "confidence": 0,
  "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
  "expirationDateTime": "2019-03-01T21:43:37.5031462+00:00",
  "externalId": "Test--8586509942679764298MS501",
  "fileHashType": "sha256",
  "fileHashValue": "aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313",
  "killChain": [],
  "malwareFamilyNames": [],
  "severity": 0,
  "tags": [],
  "targetProduct": "Azure Sentinel",
  "threatType": "WatchList",
  "tlpLevel": "green"
}
```

### <a name="response"></a><span data-ttu-id="7ba34-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ba34-129">Response</span></span>

<span data-ttu-id="7ba34-130">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7ba34-130">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="7ba34-131">Das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="7ba34-131">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7ba34-132">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="7ba34-132">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Security/tiIndicators/$entity",
    "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
    "azureTenantId": "XXXXXXXXXXXXXXXXXXXX",
    "action": "alert",
    "additionalInformation": null,
    "activityGroupNames": [],
    "confidence": 0,
    "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
