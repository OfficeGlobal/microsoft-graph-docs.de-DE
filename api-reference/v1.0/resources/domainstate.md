---
title: domainState-Ressourcentyp
description: Stellt den Status asynchroner Vorgänge dar, die in einer Domäne geplant sind.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: f24a5a9c493dc1cea16cb9038b85dc0a793bdfee
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880647"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="cafb2-103">domainState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cafb2-103">domainState resource type</span></span>

<span data-ttu-id="cafb2-104">Stellt den Status asynchroner Vorgänge dar, die in einer Domäne geplant sind.</span><span class="sxs-lookup"><span data-stu-id="cafb2-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="cafb2-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cafb2-105">Properties</span></span>

| <span data-ttu-id="cafb2-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cafb2-106">Property</span></span>   | <span data-ttu-id="cafb2-107">Typ</span><span class="sxs-lookup"><span data-stu-id="cafb2-107">Type</span></span> | <span data-ttu-id="cafb2-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cafb2-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="cafb2-109">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="cafb2-109">lastActionDateTime</span></span> | <span data-ttu-id="cafb2-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cafb2-110">DateTimeOffset</span></span> | <span data-ttu-id="cafb2-p101">Zeitstempel der letzten Aktivität. Der Wert wird aktualisiert, wenn ein Vorgang geplant, die asynchrone Aufgabe gestartet und der Vorgang abgeschlossen wird.</span><span class="sxs-lookup"><span data-stu-id="cafb2-p101">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="cafb2-113">Operation</span><span class="sxs-lookup"><span data-stu-id="cafb2-113">operation</span></span> | <span data-ttu-id="cafb2-114">String</span><span class="sxs-lookup"><span data-stu-id="cafb2-114">String</span></span> | <span data-ttu-id="cafb2-p102">Typ des asynchronen Vorgangs. Mögliche Werte sind *ForceDelete* und *Verification*</span><span class="sxs-lookup"><span data-stu-id="cafb2-p102">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="cafb2-117">status</span><span class="sxs-lookup"><span data-stu-id="cafb2-117">status</span></span> | <span data-ttu-id="cafb2-118">String</span><span class="sxs-lookup"><span data-stu-id="cafb2-118">String</span></span> | <span data-ttu-id="cafb2-119">Der aktuellen Status des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="cafb2-119">Current status of the operation.</span></span> <br> <span data-ttu-id="cafb2-120">*Scheduled*: Der Vorgang wurde geplant, aber noch nicht gestartet.</span><span class="sxs-lookup"><span data-stu-id="cafb2-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="cafb2-121">*InProgress*: Der Vorgang wurde gestartet und wird ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="cafb2-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="cafb2-122">*Failed*: Ein Fehler ist im Vorgang aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="cafb2-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cafb2-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cafb2-123">JSON representation</span></span>
<span data-ttu-id="cafb2-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cafb2-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
