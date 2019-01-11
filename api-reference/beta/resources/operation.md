---
title: Vorgang Ressourcentyp
description: Der Status der ein zeitintensiver Vorgang.
localization_priority: Normal
ms.openlocfilehash: 760aeedb67b987fc22a5eef969e2214f6dfd05b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830345"
---
# <a name="operation-resource-type"></a><span data-ttu-id="fa4d5-103">Vorgang Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fa4d5-103">operation resource type</span></span>

> <span data-ttu-id="fa4d5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fa4d5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa4d5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa4d5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa4d5-106">Der Status der ein zeitintensiver Vorgang.</span><span class="sxs-lookup"><span data-stu-id="fa4d5-106">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="fa4d5-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="fa4d5-107">Methods</span></span>

<span data-ttu-id="fa4d5-108">Keine</span><span class="sxs-lookup"><span data-stu-id="fa4d5-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="fa4d5-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fa4d5-109">Properties</span></span>

| <span data-ttu-id="fa4d5-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa4d5-110">Property</span></span>           | <span data-ttu-id="fa4d5-111">Typ</span><span class="sxs-lookup"><span data-stu-id="fa4d5-111">Type</span></span>            | <span data-ttu-id="fa4d5-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa4d5-112">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="fa4d5-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa4d5-113">createdDateTime</span></span>    | <span data-ttu-id="fa4d5-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa4d5-114">DateTimeOffset</span></span>  | <span data-ttu-id="fa4d5-115">Die Startzeit des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="fa4d5-115">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="fa4d5-116">id</span><span class="sxs-lookup"><span data-stu-id="fa4d5-116">id</span></span>                 | <span data-ttu-id="fa4d5-117">String</span><span class="sxs-lookup"><span data-stu-id="fa4d5-117">String</span></span>          | <span data-ttu-id="fa4d5-118">Die Vorgangs-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fa4d5-118">The operation id. Read-only.</span></span> <span data-ttu-id="fa4d5-119">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="fa4d5-119">Server generated.</span></span>                                  |
| <span data-ttu-id="fa4d5-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="fa4d5-120">lastActionDateTime</span></span> | <span data-ttu-id="fa4d5-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa4d5-121">DateTimeOffset</span></span>  | <span data-ttu-id="fa4d5-122">Der Zeitpunkt der letzten Aktion des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="fa4d5-122">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="fa4d5-123">status</span><span class="sxs-lookup"><span data-stu-id="fa4d5-123">status</span></span>             | <span data-ttu-id="fa4d5-124">String</span><span class="sxs-lookup"><span data-stu-id="fa4d5-124">String</span></span>          | <span data-ttu-id="fa4d5-125">Mögliche Werte: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="fa4d5-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="fa4d5-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fa4d5-126">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fa4d5-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fa4d5-127">Relationships</span></span>

<span data-ttu-id="fa4d5-128">Keine</span><span class="sxs-lookup"><span data-stu-id="fa4d5-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa4d5-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fa4d5-129">JSON representation</span></span>

<span data-ttu-id="fa4d5-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fa4d5-130">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="fa4d5-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa4d5-131">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "status": "completed"
}
```

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
