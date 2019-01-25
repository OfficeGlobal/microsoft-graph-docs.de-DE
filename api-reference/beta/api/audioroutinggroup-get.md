---
title: Abrufen von audio Routinggruppe
description: Rufen Sie die Eigenschaften und die Beziehungen eines AudioRoutingGroup-Objekts ab.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 810a27c91c5a31a970f7b279d774d12bf049210d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524037"
---
# <a name="get-audio-routing-group"></a><span data-ttu-id="6e998-103">Abrufen von audio Routinggruppe</span><span class="sxs-lookup"><span data-stu-id="6e998-103">Get audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e998-104">Rufen Sie die Eigenschaften und die Beziehungen eines [AudioRoutingGroup](../resources/audioroutinggroup.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="6e998-104">Retrieve the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e998-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6e998-105">Permissions</span></span>
<span data-ttu-id="6e998-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e998-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e998-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6e998-108">Permission type</span></span>                        | <span data-ttu-id="6e998-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6e998-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6e998-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6e998-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e998-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6e998-111">Not Supported</span></span>                               |
| <span data-ttu-id="6e998-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6e998-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e998-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6e998-113">Not Supported</span></span>                               |
| <span data-ttu-id="6e998-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6e998-114">Application</span></span>                            | <span data-ttu-id="6e998-115">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="6e998-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e998-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e998-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups/{id}
GET /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e998-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6e998-117">Optional query parameters</span></span>
<span data-ttu-id="6e998-118">Diese Methode unterstützt die [OData-Abfrage-Parameter](/graph/query-parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="6e998-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e998-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6e998-119">Request headers</span></span>
| <span data-ttu-id="6e998-120">Name</span><span class="sxs-lookup"><span data-stu-id="6e998-120">Name</span></span>          | <span data-ttu-id="6e998-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e998-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6e998-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e998-122">Authorization</span></span> | <span data-ttu-id="6e998-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6e998-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e998-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6e998-125">Request body</span></span>
<span data-ttu-id="6e998-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6e998-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e998-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e998-127">Response</span></span>
<span data-ttu-id="6e998-128">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines [AudioRoutingGroup](../resources/audioroutinggroup.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6e998-128">If successful, this method returns a `200 OK` response code and an [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e998-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6e998-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6e998-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e998-130">Request</span></span>
<span data-ttu-id="6e998-131">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="6e998-131">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroup"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="6e998-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e998-132">Response</span></span>

> <span data-ttu-id="6e998-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="6e998-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Get audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/audioroutinggroup-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
