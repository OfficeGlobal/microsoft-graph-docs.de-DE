---
title: Ressourcentyp synchronizationError
description: Stellt einen Fehler, der während der Synchronisation aufgetreten sind.
ms.openlocfilehash: a1e3725151a4e36772cd3b6079f787370f4c85dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058917"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="1287f-103">Ressourcentyp synchronizationError</span><span class="sxs-lookup"><span data-stu-id="1287f-103">synchronizationError resource type</span></span>

> <span data-ttu-id="1287f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1287f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1287f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1287f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1287f-106">Stellt einen Fehler, der während der Synchronisation aufgetreten sind.</span><span class="sxs-lookup"><span data-stu-id="1287f-106">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="1287f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1287f-107">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="1287f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1287f-108">Property</span></span>     | <span data-ttu-id="1287f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="1287f-109">Type</span></span>   |<span data-ttu-id="1287f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1287f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1287f-111">code</span><span class="sxs-lookup"><span data-stu-id="1287f-111">code</span></span>|<span data-ttu-id="1287f-112">String</span><span class="sxs-lookup"><span data-stu-id="1287f-112">String</span></span>||
|<span data-ttu-id="1287f-113">message</span><span class="sxs-lookup"><span data-stu-id="1287f-113">message</span></span>|<span data-ttu-id="1287f-114">String</span><span class="sxs-lookup"><span data-stu-id="1287f-114">String</span></span>||
|<span data-ttu-id="1287f-115">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="1287f-115">tenantActionable</span></span>|<span data-ttu-id="1287f-116">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1287f-116">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="1287f-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1287f-117">JSON representation</span></span>

<span data-ttu-id="1287f-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1287f-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->