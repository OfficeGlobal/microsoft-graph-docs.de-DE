---
title: Vorgang Ressourcentyp
description: Der Status der ein zeitintensiver Vorgang.
ms.openlocfilehash: 622a17233a25709047ea852b7df5020aee3ae343
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016511"
---
# <a name="operation-resource-type"></a><span data-ttu-id="d4860-103">Vorgang Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d4860-103">operation resource type</span></span>

<span data-ttu-id="d4860-104">Der Status der ein zeitintensiver Vorgang.</span><span class="sxs-lookup"><span data-stu-id="d4860-104">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4860-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d4860-105">JSON representation</span></span>

<span data-ttu-id="d4860-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d4860-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="d4860-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d4860-107">Properties</span></span>
| <span data-ttu-id="d4860-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4860-108">Property</span></span>     | <span data-ttu-id="d4860-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d4860-109">Type</span></span>   |<span data-ttu-id="d4860-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4860-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4860-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4860-111">createdDateTime</span></span>| <span data-ttu-id="d4860-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4860-112">DateTimeOffset</span></span> |<span data-ttu-id="d4860-113">Die Startzeit des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="d4860-113">The start time of the operation.</span></span>|
|<span data-ttu-id="d4860-114">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="d4860-114">lastActionDateTime</span></span>| <span data-ttu-id="d4860-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4860-115">DateTimeOffset</span></span> |<span data-ttu-id="d4860-116">Der Zeitpunkt der letzten Aktion des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="d4860-116">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="d4860-117">status</span><span class="sxs-lookup"><span data-stu-id="d4860-117">status</span></span>|<span data-ttu-id="d4860-118">operationStatus</span><span class="sxs-lookup"><span data-stu-id="d4860-118">operationStatus</span></span>|<span data-ttu-id="d4860-119">Der aktuellen Status des Vorgangs: `notStarted`, `running`, `completed`, `failed`</span><span class="sxs-lookup"><span data-stu-id="d4860-119">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
