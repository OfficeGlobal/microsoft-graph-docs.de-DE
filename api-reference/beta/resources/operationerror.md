---
title: Ressourcentyp operationError
description: Fehler in TeamsAsyncOperation beschreibt.
localization_priority: Normal
ms.openlocfilehash: 423f426df92e99754af0abf4c9c8088eea61d5ea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890293"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="f89c7-103">Ressourcentyp operationError</span><span class="sxs-lookup"><span data-stu-id="f89c7-103">operationError resource type</span></span>

> <span data-ttu-id="f89c7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f89c7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f89c7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f89c7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f89c7-106">Fehler in [TeamsAsyncOperation](teamsasyncoperation.md)beschreibt.</span><span class="sxs-lookup"><span data-stu-id="f89c7-106">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="f89c7-107">OperationError Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f89c7-107">operationError Properties</span></span>
| <span data-ttu-id="f89c7-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f89c7-108">Property</span></span>     | <span data-ttu-id="f89c7-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f89c7-109">Type</span></span>   |<span data-ttu-id="f89c7-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f89c7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f89c7-111">code</span><span class="sxs-lookup"><span data-stu-id="f89c7-111">code</span></span>|<span data-ttu-id="f89c7-112">Zeichenfolge (schreibgeschützt)</span><span class="sxs-lookup"><span data-stu-id="f89c7-112">string (readonly)</span></span>|<span data-ttu-id="f89c7-113">Fehlercode Vorgang.</span><span class="sxs-lookup"><span data-stu-id="f89c7-113">Operation error code.</span></span>|
|<span data-ttu-id="f89c7-114">message</span><span class="sxs-lookup"><span data-stu-id="f89c7-114">message</span></span>|<span data-ttu-id="f89c7-115">Zeichenfolge (schreibgeschützt)</span><span class="sxs-lookup"><span data-stu-id="f89c7-115">string (readonly)</span></span>|<span data-ttu-id="f89c7-116">Vorgang Fehlermeldung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f89c7-116">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f89c7-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f89c7-117">JSON representation</span></span>

<span data-ttu-id="f89c7-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f89c7-118">The following is a JSON representation of the resource.</span></span>

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
