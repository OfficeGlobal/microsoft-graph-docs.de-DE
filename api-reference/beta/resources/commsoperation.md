---
title: Ressourcentyp commsOperation
description: Der Status der bestimmte langer Vorgänge.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5a82020741033f81d5a4394f2e32b3f0f76a6e03
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575646"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="c6bbe-103">Ressourcentyp commsOperation</span><span class="sxs-lookup"><span data-stu-id="c6bbe-103">commsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6bbe-104">Der Status der bestimmte langer Vorgänge.</span><span class="sxs-lookup"><span data-stu-id="c6bbe-104">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="c6bbe-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="c6bbe-105">Methods</span></span>
<span data-ttu-id="c6bbe-106">Keine</span><span class="sxs-lookup"><span data-stu-id="c6bbe-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="c6bbe-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c6bbe-107">Properties</span></span>

| <span data-ttu-id="c6bbe-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c6bbe-108">Property</span></span>           | <span data-ttu-id="c6bbe-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c6bbe-109">Type</span></span>                        | <span data-ttu-id="c6bbe-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6bbe-110">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="c6bbe-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="c6bbe-111">clientContext</span></span>      | <span data-ttu-id="c6bbe-112">String</span><span class="sxs-lookup"><span data-stu-id="c6bbe-112">String</span></span>                      | <span data-ttu-id="c6bbe-113">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="c6bbe-113">The client context.</span></span>                                                             |
| <span data-ttu-id="c6bbe-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6bbe-114">createdDateTime</span></span>    | <span data-ttu-id="c6bbe-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6bbe-115">DateTimeOffset</span></span>              | <span data-ttu-id="c6bbe-116">Die Startzeit des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="c6bbe-116">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="c6bbe-117">id</span><span class="sxs-lookup"><span data-stu-id="c6bbe-117">id</span></span>                 | <span data-ttu-id="c6bbe-118">Zeichenfolge (ID)</span><span class="sxs-lookup"><span data-stu-id="c6bbe-118">String (identifier)</span></span>         | <span data-ttu-id="c6bbe-119">Die Vorgangs-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c6bbe-119">The operation id. Read-only.</span></span> <span data-ttu-id="c6bbe-120">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="c6bbe-120">Server generated.</span></span>                                  |
| <span data-ttu-id="c6bbe-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="c6bbe-121">lastActionDateTime</span></span> | <span data-ttu-id="c6bbe-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6bbe-122">DateTimeOffset</span></span>              | <span data-ttu-id="c6bbe-123">Der Zeitpunkt der letzten Aktion des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="c6bbe-123">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="c6bbe-124">errorInfo</span><span class="sxs-lookup"><span data-stu-id="c6bbe-124">errorInfo</span></span>          | [<span data-ttu-id="c6bbe-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c6bbe-125">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="c6bbe-126">Informationen zu den Ergebnissen.</span><span class="sxs-lookup"><span data-stu-id="c6bbe-126">The result information.</span></span> <span data-ttu-id="c6bbe-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c6bbe-127">Read-only.</span></span> <span data-ttu-id="c6bbe-128">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="c6bbe-128">Server generated.</span></span>                            |
| <span data-ttu-id="c6bbe-129">status</span><span class="sxs-lookup"><span data-stu-id="c6bbe-129">status</span></span>             | <span data-ttu-id="c6bbe-130">operationStatus</span><span class="sxs-lookup"><span data-stu-id="c6bbe-130">operationStatus</span></span>             | <span data-ttu-id="c6bbe-131">Mögliche Werte: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="c6bbe-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="c6bbe-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c6bbe-132">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c6bbe-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c6bbe-133">Relationships</span></span>
<span data-ttu-id="c6bbe-134">Keine</span><span class="sxs-lookup"><span data-stu-id="c6bbe-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6bbe-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c6bbe-135">JSON representation</span></span>

<span data-ttu-id="c6bbe-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c6bbe-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "errorInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "operationStatus"
}
```

## <a name="example"></a><span data-ttu-id="c6bbe-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c6bbe-137">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo",
    "code": "200"
  },
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/commsoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
