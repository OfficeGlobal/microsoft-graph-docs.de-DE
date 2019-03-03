---
title: 'tiIndicator: deleteTiIndicators'
description: Löschen Sie mehrere Threat Intelligence-Indikatoren (TI) in einer Anforderung anstelle mehrerer Anforderungen.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 49475f15520f02cc36bb1bf37af9a5849a8ee245
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366959"
---
# <a name="tiindicator-deletetiindicators"></a><span data-ttu-id="77a44-103">tiIndicator: deleteTiIndicators</span><span class="sxs-lookup"><span data-stu-id="77a44-103">tiIndicator: deleteTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77a44-104">Löschen Sie mehrere Threat Intelligence-Indikatoren (TI) in einer Anforderung anstelle mehrerer Anforderungen.</span><span class="sxs-lookup"><span data-stu-id="77a44-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="77a44-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="77a44-105">Permissions</span></span>

<span data-ttu-id="77a44-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77a44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="77a44-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="77a44-108">Permission type</span></span> | <span data-ttu-id="77a44-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="77a44-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="77a44-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="77a44-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="77a44-111">ThreatIndicators. ReadWrite. OwnedBy</span><span class="sxs-lookup"><span data-stu-id="77a44-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="77a44-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="77a44-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77a44-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77a44-113">Not supported.</span></span> |
| <span data-ttu-id="77a44-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="77a44-114">Application</span></span>                            | <span data-ttu-id="77a44-115">ThreatIndicators. ReadWrite. OwnedBy</span><span class="sxs-lookup"><span data-stu-id="77a44-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="77a44-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="77a44-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="77a44-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="77a44-117">Request headers</span></span>

| <span data-ttu-id="77a44-118">Name</span><span class="sxs-lookup"><span data-stu-id="77a44-118">Name</span></span>          | <span data-ttu-id="77a44-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77a44-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="77a44-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="77a44-120">Authorization</span></span> | <span data-ttu-id="77a44-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="77a44-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="77a44-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="77a44-122">Request body</span></span>

<span data-ttu-id="77a44-123">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="77a44-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="77a44-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="77a44-124">Parameter</span></span>    | <span data-ttu-id="77a44-125">Typ</span><span class="sxs-lookup"><span data-stu-id="77a44-125">Type</span></span>        | <span data-ttu-id="77a44-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77a44-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="77a44-127">Wert</span><span class="sxs-lookup"><span data-stu-id="77a44-127">value</span></span>|<span data-ttu-id="77a44-128">String collection</span><span class="sxs-lookup"><span data-stu-id="77a44-128">String collection</span></span>| <span data-ttu-id="77a44-129">Sammlung von tiIndicator `id`s, die gelöscht werden sollen.</span><span class="sxs-lookup"><span data-stu-id="77a44-129">Collection of tiIndicator `id`s to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="77a44-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="77a44-130">Response</span></span>

<span data-ttu-id="77a44-131">Bei erfolgreicher Ausführung gibt diese Methode `200, OK` den Antwortcode und ein [resultInfo](../resources/resultinfo.md) -Auflistungsobjekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="77a44-131">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="77a44-132">Beispiele</span><span class="sxs-lookup"><span data-stu-id="77a44-132">Examples</span></span>

<span data-ttu-id="77a44-133">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="77a44-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="77a44-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="77a44-134">Request</span></span>

<span data-ttu-id="77a44-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="77a44-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicators"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicators
Content-type: application/json

{
  "value": [
    "id-value1",
    "id-value2"
  ]
}
```

### <a name="response"></a><span data-ttu-id="77a44-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="77a44-136">Response</span></span>

<span data-ttu-id="77a44-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="77a44-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="77a44-138">Das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="77a44-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="77a44-139">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="77a44-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resultInfo",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
{
  "value": [
    {
      "code": "code-value",
      "message": "message-value",
      "subCode": "subCode-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: deleteTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
