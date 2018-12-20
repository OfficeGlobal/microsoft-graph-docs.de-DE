---
title: Ressourcentyp commsOperation
description: Der Status der bestimmte langer Vorgänge.
author: VinodRavichandran
ms.openlocfilehash: 09d3f81e8f6307850d94cfab43f98426dae47a5f
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380352"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="781cb-103">Ressourcentyp commsOperation</span><span class="sxs-lookup"><span data-stu-id="781cb-103">commsOperation resource type</span></span>

> <span data-ttu-id="781cb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="781cb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="781cb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="781cb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="781cb-106">Der Status der bestimmte langer Vorgänge.</span><span class="sxs-lookup"><span data-stu-id="781cb-106">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="781cb-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="781cb-107">Methods</span></span>
<span data-ttu-id="781cb-108">Keine</span><span class="sxs-lookup"><span data-stu-id="781cb-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="781cb-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="781cb-109">Properties</span></span>

| <span data-ttu-id="781cb-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="781cb-110">Property</span></span>           | <span data-ttu-id="781cb-111">Typ</span><span class="sxs-lookup"><span data-stu-id="781cb-111">Type</span></span>                        | <span data-ttu-id="781cb-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="781cb-112">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="781cb-113">clientContext</span><span class="sxs-lookup"><span data-stu-id="781cb-113">clientContext</span></span>      | <span data-ttu-id="781cb-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="781cb-114">String</span></span>                      | <span data-ttu-id="781cb-115">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="781cb-115">The client context.</span></span>                                                             |
| <span data-ttu-id="781cb-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="781cb-116">createdDateTime</span></span>    | <span data-ttu-id="781cb-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="781cb-117">DateTimeOffset</span></span>              | <span data-ttu-id="781cb-118">Die Startzeit des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="781cb-118">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="781cb-119">id</span><span class="sxs-lookup"><span data-stu-id="781cb-119">id</span></span>                 | <span data-ttu-id="781cb-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="781cb-120">String</span></span>                      | <span data-ttu-id="781cb-121">Die Vorgangs-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="781cb-121">The operation id. Read-only.</span></span> <span data-ttu-id="781cb-122">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="781cb-122">Server generated.</span></span>                                  |
| <span data-ttu-id="781cb-123">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="781cb-123">lastActionDateTime</span></span> | <span data-ttu-id="781cb-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="781cb-124">DateTimeOffset</span></span>              | <span data-ttu-id="781cb-125">Der Zeitpunkt der letzten Aktion des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="781cb-125">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="781cb-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="781cb-126">resultInfo</span></span>         | [<span data-ttu-id="781cb-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="781cb-127">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="781cb-128">Informationen zu den Ergebnissen.</span><span class="sxs-lookup"><span data-stu-id="781cb-128">The result information.</span></span> <span data-ttu-id="781cb-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="781cb-129">Read-only.</span></span> <span data-ttu-id="781cb-130">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="781cb-130">Server generated.</span></span>                            |
| <span data-ttu-id="781cb-131">status</span><span class="sxs-lookup"><span data-stu-id="781cb-131">status</span></span>             | <span data-ttu-id="781cb-132">String</span><span class="sxs-lookup"><span data-stu-id="781cb-132">String</span></span>                      | <span data-ttu-id="781cb-133">Mögliche Werte: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="781cb-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="781cb-134">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="781cb-134">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="781cb-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="781cb-135">Relationships</span></span>
<span data-ttu-id="781cb-136">Keine</span><span class="sxs-lookup"><span data-stu-id="781cb-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="781cb-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="781cb-137">JSON representation</span></span>

<span data-ttu-id="781cb-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="781cb-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resultInfo": { "@odata.type": "#microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="781cb-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="781cb-139">Example</span></span>

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
    "@odata.type": "#microsoft.graph.resultInfo",
    "code": "200"
  },
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
