---
title: workbookSessionInfo-Ressourcentyp
description: Enthält Informationen zu Arbeitsmappensitzungen.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 900ebdcefbdfa83e7b72b1c926a441f1c497626a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826929"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="0cb4f-103">workbookSessionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0cb4f-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="0cb4f-104">Enthält Informationen zu Arbeitsmappensitzungen.</span><span class="sxs-lookup"><span data-stu-id="0cb4f-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0cb4f-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0cb4f-105">JSON representation</span></span>

<span data-ttu-id="0cb4f-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0cb4f-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a><span data-ttu-id="0cb4f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0cb4f-107">Properties</span></span>

| <span data-ttu-id="0cb4f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0cb4f-108">Property</span></span> | <span data-ttu-id="0cb4f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="0cb4f-109">Type</span></span>  | <span data-ttu-id="0cb4f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0cb4f-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="0cb4f-111">id</span><span class="sxs-lookup"><span data-stu-id="0cb4f-111">id</span></span>  | <span data-ttu-id="0cb4f-112">string</span><span class="sxs-lookup"><span data-stu-id="0cb4f-112">string</span></span> | <span data-ttu-id="0cb4f-113">Die ID der Arbeitsmappensitzung.</span><span class="sxs-lookup"><span data-stu-id="0cb4f-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="0cb4f-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="0cb4f-114">persistChanges</span></span> | <span data-ttu-id="0cb4f-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cb4f-115">boolean</span></span> |  <span data-ttu-id="0cb4f-116">`true` für eine beständige Sitzung</span><span class="sxs-lookup"><span data-stu-id="0cb4f-116">`true` for persistent session.</span></span> <span data-ttu-id="0cb4f-117">`false` für eine nicht-beständige Sitzung (Ansichtsmodus)</span><span class="sxs-lookup"><span data-stu-id="0cb4f-117">`false` for non-persistent session (view mode)</span></span> |

