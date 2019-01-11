---
title: Vorgang Ressourcentyp
description: Der Status der ein zeitintensiver Vorgang.
localization_priority: Normal
ms.openlocfilehash: 4f2e2c9a6fb9eb6d26a3511c637e79822919e2f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884966"
---
# <a name="operation-resource-type"></a><span data-ttu-id="e0b6d-103">Vorgang Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e0b6d-103">operation resource type</span></span>

<span data-ttu-id="e0b6d-104">Der Status der ein zeitintensiver Vorgang.</span><span class="sxs-lookup"><span data-stu-id="e0b6d-104">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0b6d-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e0b6d-105">JSON representation</span></span>

<span data-ttu-id="e0b6d-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e0b6d-106">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}

```
## <a name="properties"></a><span data-ttu-id="e0b6d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e0b6d-107">Properties</span></span>
| <span data-ttu-id="e0b6d-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e0b6d-108">Property</span></span>     | <span data-ttu-id="e0b6d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e0b6d-109">Type</span></span>   |<span data-ttu-id="e0b6d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0b6d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0b6d-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0b6d-111">createdDateTime</span></span>| <span data-ttu-id="e0b6d-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0b6d-112">DateTimeOffset</span></span> |<span data-ttu-id="e0b6d-113">Die Startzeit des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="e0b6d-113">The start time of the operation.</span></span>|
|<span data-ttu-id="e0b6d-114">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="e0b6d-114">lastActionDateTime</span></span>| <span data-ttu-id="e0b6d-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0b6d-115">DateTimeOffset</span></span> |<span data-ttu-id="e0b6d-116">Der Zeitpunkt der letzten Aktion des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="e0b6d-116">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="e0b6d-117">status</span><span class="sxs-lookup"><span data-stu-id="e0b6d-117">status</span></span>|<span data-ttu-id="e0b6d-118">operationStatus</span><span class="sxs-lookup"><span data-stu-id="e0b6d-118">operationStatus</span></span>|<span data-ttu-id="e0b6d-119">Der aktuellen Status des Vorgangs: `notStarted`, `running`, `completed`, `failed`</span><span class="sxs-lookup"><span data-stu-id="e0b6d-119">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
