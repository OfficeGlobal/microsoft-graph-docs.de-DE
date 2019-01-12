---
title: workbookSessionInfo-Ressourcentyp
description: Enthält Informationen zu Arbeitsmappensitzungen.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 502781c4049c9451f5ed67ff97222abf4df462d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960273"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="bd14f-103">workbookSessionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bd14f-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="bd14f-104">Enthält Informationen zu Arbeitsmappensitzungen.</span><span class="sxs-lookup"><span data-stu-id="bd14f-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="bd14f-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bd14f-105">JSON representation</span></span>

<span data-ttu-id="bd14f-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bd14f-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="bd14f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bd14f-107">Properties</span></span>

| <span data-ttu-id="bd14f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd14f-108">Property</span></span> | <span data-ttu-id="bd14f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="bd14f-109">Type</span></span>  | <span data-ttu-id="bd14f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd14f-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="bd14f-111">id</span><span class="sxs-lookup"><span data-stu-id="bd14f-111">id</span></span>  | <span data-ttu-id="bd14f-112">string</span><span class="sxs-lookup"><span data-stu-id="bd14f-112">string</span></span> | <span data-ttu-id="bd14f-113">Die ID der Arbeitsmappensitzung.</span><span class="sxs-lookup"><span data-stu-id="bd14f-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="bd14f-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="bd14f-114">persistChanges</span></span> | <span data-ttu-id="bd14f-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd14f-115">boolean</span></span> |  <span data-ttu-id="bd14f-116">`true` für eine beständige Sitzung</span><span class="sxs-lookup"><span data-stu-id="bd14f-116">`true` for persistent session.</span></span> <span data-ttu-id="bd14f-117">`false` für eine nicht-beständige Sitzung (Ansichtsmodus)</span><span class="sxs-lookup"><span data-stu-id="bd14f-117">`false` for non-persistent session (view mode)</span></span> |

