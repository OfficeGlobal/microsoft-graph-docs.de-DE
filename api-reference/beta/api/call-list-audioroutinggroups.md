---
title: Liste audio Routinggruppen
description: Abrufen einer Liste von **AudioRoutingGroup** -Objekten.
author: VinodRavichandran
ms.openlocfilehash: 7ed00bbd3d000e71afe55a5e663408139174640b
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380135"
---
# <a name="list-audio-routing-groups"></a><span data-ttu-id="9d5c5-103">Liste audio Routinggruppen</span><span class="sxs-lookup"><span data-stu-id="9d5c5-103">List audio routing groups</span></span>

> <span data-ttu-id="9d5c5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9d5c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d5c5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9d5c5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d5c5-106">Abrufen einer Liste von **AudioRoutingGroup** -Objekten.</span><span class="sxs-lookup"><span data-stu-id="9d5c5-106">Retrieve a list of **audioRoutingGroup** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d5c5-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9d5c5-107">Permissions</span></span>
<span data-ttu-id="9d5c5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d5c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9d5c5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9d5c5-110">Permission type</span></span>                        | <span data-ttu-id="9d5c5-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9d5c5-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9d5c5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9d5c5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9d5c5-113">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9d5c5-113">Not Supported.</span></span>                               |
| <span data-ttu-id="9d5c5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9d5c5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d5c5-115">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9d5c5-115">Not Supported.</span></span>                               |
| <span data-ttu-id="9d5c5-116">Application</span><span class="sxs-lookup"><span data-stu-id="9d5c5-116">Application</span></span>     | <span data-ttu-id="9d5c5-117">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="9d5c5-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d5c5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d5c5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups
GET /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9d5c5-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9d5c5-119">Optional query parameters</span></span>
<span data-ttu-id="9d5c5-120">Diese Methode unterstützt die [OData-Abfrage-Parameter](/graph/query-parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="9d5c5-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d5c5-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9d5c5-121">Request headers</span></span>
| <span data-ttu-id="9d5c5-122">Name</span><span class="sxs-lookup"><span data-stu-id="9d5c5-122">Name</span></span>          | <span data-ttu-id="9d5c5-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d5c5-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9d5c5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d5c5-124">Authorization</span></span> | <span data-ttu-id="9d5c5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9d5c5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d5c5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9d5c5-127">Request body</span></span>
<span data-ttu-id="9d5c5-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9d5c5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d5c5-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d5c5-129">Response</span></span>
<span data-ttu-id="9d5c5-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AudioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="9d5c5-130">If successful, this method returns a `200 OK` response code and a collection of [audioRoutingGroup](../resources/audioroutinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d5c5-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9d5c5-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9d5c5-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d5c5-132">Request</span></span>
<span data-ttu-id="9d5c5-133">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="9d5c5-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroups"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
```

##### <a name="response"></a><span data-ttu-id="9d5c5-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d5c5-134">Response</span></span>

> <span data-ttu-id="9d5c5-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="9d5c5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup",
  "isCollection": true 
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List audioRoutingGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
