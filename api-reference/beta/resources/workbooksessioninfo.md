---
title: workbookSessionInfo-Ressourcentyp
description: Enthält Informationen zu Arbeitsmappensitzungen.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a2975fdf58d0f1d3a72f1f76853125d0a98bb485
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962450"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="e865c-103">workbookSessionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e865c-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="e865c-104">Enthält Informationen zu Arbeitsmappensitzungen.</span><span class="sxs-lookup"><span data-stu-id="e865c-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e865c-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e865c-105">JSON representation</span></span>

<span data-ttu-id="e865c-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e865c-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="e865c-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e865c-107">Properties</span></span>

| <span data-ttu-id="e865c-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e865c-108">Property</span></span> | <span data-ttu-id="e865c-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e865c-109">Type</span></span>  | <span data-ttu-id="e865c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e865c-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="e865c-111">id</span><span class="sxs-lookup"><span data-stu-id="e865c-111">id</span></span>  | <span data-ttu-id="e865c-112">string</span><span class="sxs-lookup"><span data-stu-id="e865c-112">string</span></span> | <span data-ttu-id="e865c-113">Die ID der Arbeitsmappensitzung.</span><span class="sxs-lookup"><span data-stu-id="e865c-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="e865c-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="e865c-114">persistChanges</span></span> | <span data-ttu-id="e865c-115">string</span><span class="sxs-lookup"><span data-stu-id="e865c-115">string</span></span> |  <span data-ttu-id="e865c-116">`true` für eine beständige Sitzung</span><span class="sxs-lookup"><span data-stu-id="e865c-116">`true` for persistent session.</span></span> <span data-ttu-id="e865c-117">`false` für eine nicht-beständige Sitzung (Ansichtsmodus)</span><span class="sxs-lookup"><span data-stu-id="e865c-117">`false` for non-persistent session (view mode)</span></span> |

