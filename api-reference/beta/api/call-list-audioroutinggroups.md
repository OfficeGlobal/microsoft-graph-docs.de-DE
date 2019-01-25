---
title: Liste audio Routinggruppen
description: Abrufen einer Liste von **AudioRoutingGroup** -Objekten.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 02a782af2bb7690cc55dd3a4632aeb0cf93734da
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518527"
---
# <a name="list-audio-routing-groups"></a><span data-ttu-id="9d158-103">Liste audio Routinggruppen</span><span class="sxs-lookup"><span data-stu-id="9d158-103">List audio routing groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d158-104">Abrufen einer Liste von **AudioRoutingGroup** -Objekten.</span><span class="sxs-lookup"><span data-stu-id="9d158-104">Retrieve a list of **audioRoutingGroup** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d158-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9d158-105">Permissions</span></span>
<span data-ttu-id="9d158-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d158-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9d158-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9d158-108">Permission type</span></span>                        | <span data-ttu-id="9d158-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9d158-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9d158-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9d158-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9d158-111">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9d158-111">Not Supported.</span></span>                               |
| <span data-ttu-id="9d158-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9d158-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d158-113">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9d158-113">Not Supported.</span></span>                               |
| <span data-ttu-id="9d158-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9d158-114">Application</span></span>     | <span data-ttu-id="9d158-115">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="9d158-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d158-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d158-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups
GET /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9d158-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9d158-117">Optional query parameters</span></span>
<span data-ttu-id="9d158-118">Diese Methode unterstützt die [OData-Abfrage-Parameter](/graph/query-parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="9d158-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d158-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9d158-119">Request headers</span></span>
| <span data-ttu-id="9d158-120">Name</span><span class="sxs-lookup"><span data-stu-id="9d158-120">Name</span></span>          | <span data-ttu-id="9d158-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d158-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9d158-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d158-122">Authorization</span></span> | <span data-ttu-id="9d158-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9d158-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d158-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9d158-125">Request body</span></span>
<span data-ttu-id="9d158-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9d158-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d158-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d158-127">Response</span></span>
<span data-ttu-id="9d158-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AudioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="9d158-128">If successful, this method returns a `200 OK` response code and a collection of [audioRoutingGroup](../resources/audioroutinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d158-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9d158-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9d158-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d158-130">Request</span></span>
<span data-ttu-id="9d158-131">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="9d158-131">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroups"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
```

##### <a name="response"></a><span data-ttu-id="9d158-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d158-132">Response</span></span>

> <span data-ttu-id="9d158-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="9d158-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List audioRoutingGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-list-audioroutinggroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
