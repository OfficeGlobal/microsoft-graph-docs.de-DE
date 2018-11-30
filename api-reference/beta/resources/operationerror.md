---
title: Ressourcentyp operationError
description: Fehler in TeamsAsyncOperation beschreibt.
ms.openlocfilehash: 0207f490328d377fedab72d2a5300baaf3645150
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060320"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="42e34-103">Ressourcentyp operationError</span><span class="sxs-lookup"><span data-stu-id="42e34-103">operationError resource type</span></span>

> <span data-ttu-id="42e34-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="42e34-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42e34-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="42e34-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="42e34-106">Fehler in [TeamsAsyncOperation](teamsasyncoperation.md)beschreibt.</span><span class="sxs-lookup"><span data-stu-id="42e34-106">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="42e34-107">OperationError Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="42e34-107">operationError Properties</span></span>
| <span data-ttu-id="42e34-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="42e34-108">Property</span></span>     | <span data-ttu-id="42e34-109">Typ</span><span class="sxs-lookup"><span data-stu-id="42e34-109">Type</span></span>   |<span data-ttu-id="42e34-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42e34-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42e34-111">code</span><span class="sxs-lookup"><span data-stu-id="42e34-111">code</span></span>|<span data-ttu-id="42e34-112">Zeichenfolge (schreibgeschützt)</span><span class="sxs-lookup"><span data-stu-id="42e34-112">string (readonly)</span></span>|<span data-ttu-id="42e34-113">Fehlercode Vorgang.</span><span class="sxs-lookup"><span data-stu-id="42e34-113">Operation error code.</span></span>|
|<span data-ttu-id="42e34-114">message</span><span class="sxs-lookup"><span data-stu-id="42e34-114">message</span></span>|<span data-ttu-id="42e34-115">Zeichenfolge (schreibgeschützt)</span><span class="sxs-lookup"><span data-stu-id="42e34-115">string (readonly)</span></span>|<span data-ttu-id="42e34-116">Vorgang Fehlermeldung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="42e34-116">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42e34-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="42e34-117">JSON representation</span></span>

<span data-ttu-id="42e34-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="42e34-118">The following is a JSON representation of the resource.</span></span>

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
