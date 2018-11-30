---
title: Ressourcentyp operationError
description: Fehler in TeamsAsyncOperation beschreibt.
ms.openlocfilehash: bcd8c989c4c69336165ef1ca29e1d114d524aa9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018995"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="cd2ea-103">Ressourcentyp operationError</span><span class="sxs-lookup"><span data-stu-id="cd2ea-103">operationError resource type</span></span>



<span data-ttu-id="cd2ea-104">Fehler in [TeamsAsyncOperation](teamsasyncoperation.md)beschreibt.</span><span class="sxs-lookup"><span data-stu-id="cd2ea-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="cd2ea-105">OperationError Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cd2ea-105">operationError Properties</span></span>
| <span data-ttu-id="cd2ea-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cd2ea-106">Property</span></span>     | <span data-ttu-id="cd2ea-107">Typ</span><span class="sxs-lookup"><span data-stu-id="cd2ea-107">Type</span></span>   |<span data-ttu-id="cd2ea-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd2ea-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd2ea-109">code</span><span class="sxs-lookup"><span data-stu-id="cd2ea-109">code</span></span>|<span data-ttu-id="cd2ea-110">Zeichenfolge (schreibgeschützt)</span><span class="sxs-lookup"><span data-stu-id="cd2ea-110">string (readonly)</span></span>|<span data-ttu-id="cd2ea-111">Fehlercode Vorgang.</span><span class="sxs-lookup"><span data-stu-id="cd2ea-111">Operation error code.</span></span>|
|<span data-ttu-id="cd2ea-112">message</span><span class="sxs-lookup"><span data-stu-id="cd2ea-112">message</span></span>|<span data-ttu-id="cd2ea-113">Zeichenfolge (schreibgeschützt)</span><span class="sxs-lookup"><span data-stu-id="cd2ea-113">string (readonly)</span></span>|<span data-ttu-id="cd2ea-114">Vorgang Fehlermeldung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="cd2ea-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd2ea-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cd2ea-115">JSON representation</span></span>

<span data-ttu-id="cd2ea-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cd2ea-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
