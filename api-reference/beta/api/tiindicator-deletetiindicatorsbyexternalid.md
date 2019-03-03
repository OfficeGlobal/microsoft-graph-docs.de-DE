---
title: 'tiIndicator: deleteTiIndicatorsByExternalId'
description: Löschen Sie mehrere Threat Intelligence (TI)-Indikatoren in einer Anforderung anstelle mehrerer Anforderungen, und die Anforderung enthält Externe IDs anstelle von IDs.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 82cdd0d9688e778982244a06a2a2e5d558d25807
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366945"
---
# <a name="tiindicator-deletetiindicatorsbyexternalid"></a><span data-ttu-id="83a94-103">tiIndicator: deleteTiIndicatorsByExternalId</span><span class="sxs-lookup"><span data-stu-id="83a94-103">tiIndicator: deleteTiIndicatorsByExternalId</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83a94-104">Löschen Sie mehrere Threat Intelligence (TI)-Indikatoren in einer Anforderung anstelle mehrerer Anforderungen, wenn die Anforderung externe IDs anstelle von IDs enthält.</span><span class="sxs-lookup"><span data-stu-id="83a94-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests, when the request contains external IDs instead of IDs.</span></span>

## <a name="permissions"></a><span data-ttu-id="83a94-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="83a94-105">Permissions</span></span>

<span data-ttu-id="83a94-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83a94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83a94-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="83a94-108">Permission type</span></span>  | <span data-ttu-id="83a94-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="83a94-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="83a94-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="83a94-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="83a94-111">ThreatIndicators. ReadWrite. OwnedBy</span><span class="sxs-lookup"><span data-stu-id="83a94-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="83a94-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="83a94-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83a94-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="83a94-113">Not supported.</span></span> |
| <span data-ttu-id="83a94-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="83a94-114">Application</span></span>                            | <span data-ttu-id="83a94-115">ThreatIndicators. ReadWrite. OwnedBy</span><span class="sxs-lookup"><span data-stu-id="83a94-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="83a94-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="83a94-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicatorsByExternalId
```

## <a name="request-headers"></a><span data-ttu-id="83a94-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="83a94-117">Request headers</span></span>

| <span data-ttu-id="83a94-118">Name</span><span class="sxs-lookup"><span data-stu-id="83a94-118">Name</span></span>          | <span data-ttu-id="83a94-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83a94-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="83a94-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="83a94-120">Authorization</span></span> | <span data-ttu-id="83a94-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="83a94-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="83a94-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="83a94-122">Request body</span></span>

<span data-ttu-id="83a94-123">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="83a94-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="83a94-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="83a94-124">Parameter</span></span>    | <span data-ttu-id="83a94-125">Typ</span><span class="sxs-lookup"><span data-stu-id="83a94-125">Type</span></span>        | <span data-ttu-id="83a94-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83a94-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="83a94-127">Wert</span><span class="sxs-lookup"><span data-stu-id="83a94-127">value</span></span>|<span data-ttu-id="83a94-128">String collection</span><span class="sxs-lookup"><span data-stu-id="83a94-128">String collection</span></span>| <span data-ttu-id="83a94-129">Auflistung der zu löschenden TiIndicator-Objekte. \*\*\*\* `externalIds`</span><span class="sxs-lookup"><span data-stu-id="83a94-129">Collection of `externalIds` of the **tiIndicator** objects to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="83a94-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="83a94-130">Response</span></span>

<span data-ttu-id="83a94-131">Bei erfolgreicher Ausführung gibt diese Methode `200 OK` den Antwortcode und ein [resultInfo](../resources/resultinfo.md) -Auflistungsobjekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="83a94-131">If successful, this method returns `200 OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83a94-132">Beispiele</span><span class="sxs-lookup"><span data-stu-id="83a94-132">Examples</span></span>

<span data-ttu-id="83a94-133">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="83a94-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="83a94-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="83a94-134">Request</span></span>

<span data-ttu-id="83a94-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="83a94-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicatorsbyexternalid"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicatorsByExternalId
Content-type: application/json

{
  "value": [
    "externalId-value1",
    "externalId-value2"
  ]
}
```

### <a name="response"></a><span data-ttu-id="83a94-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="83a94-136">Response</span></span>

<span data-ttu-id="83a94-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="83a94-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="83a94-138">Das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="83a94-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="83a94-139">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="83a94-139">All the properties will be returned from an actual call.</span></span>

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
  "description": "tiIndicator: deleteTiIndicatorsByExternalId",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
