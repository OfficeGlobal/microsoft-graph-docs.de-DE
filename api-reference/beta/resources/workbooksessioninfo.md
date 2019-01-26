---
title: workbookSessionInfo-Ressourcentyp
description: Enthält Informationen zu Arbeitsmappensitzungen.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 502781c4049c9451f5ed67ff97222abf4df462d7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575618"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="e86d9-103">workbookSessionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e86d9-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="e86d9-104">Enthält Informationen zu Arbeitsmappensitzungen.</span><span class="sxs-lookup"><span data-stu-id="e86d9-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e86d9-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e86d9-105">JSON representation</span></span>

<span data-ttu-id="e86d9-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e86d9-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="e86d9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e86d9-107">Properties</span></span>

| <span data-ttu-id="e86d9-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e86d9-108">Property</span></span> | <span data-ttu-id="e86d9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e86d9-109">Type</span></span>  | <span data-ttu-id="e86d9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e86d9-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="e86d9-111">id</span><span class="sxs-lookup"><span data-stu-id="e86d9-111">id</span></span>  | <span data-ttu-id="e86d9-112">string</span><span class="sxs-lookup"><span data-stu-id="e86d9-112">string</span></span> | <span data-ttu-id="e86d9-113">Die ID der Arbeitsmappensitzung.</span><span class="sxs-lookup"><span data-stu-id="e86d9-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="e86d9-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="e86d9-114">persistChanges</span></span> | <span data-ttu-id="e86d9-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e86d9-115">boolean</span></span> |  <span data-ttu-id="e86d9-116">`true` für eine beständige Sitzung</span><span class="sxs-lookup"><span data-stu-id="e86d9-116">`true` for persistent session.</span></span> <span data-ttu-id="e86d9-117">`false` für eine nicht-beständige Sitzung (Ansichtsmodus)</span><span class="sxs-lookup"><span data-stu-id="e86d9-117">`false` for non-persistent session (view mode)</span></span> |

