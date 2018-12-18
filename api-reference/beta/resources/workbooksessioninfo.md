---
title: workbookSessionInfo-Ressourcentyp
description: Enthält Informationen zu Arbeitsmappensitzungen.
author: lumine2008
ms.openlocfilehash: 5a86fd4dfd653f16445eeccad8478db56db0ac5f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316842"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="f871b-103">workbookSessionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f871b-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="f871b-104">Enthält Informationen zu Arbeitsmappensitzungen.</span><span class="sxs-lookup"><span data-stu-id="f871b-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f871b-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f871b-105">JSON representation</span></span>

<span data-ttu-id="f871b-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f871b-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="f871b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f871b-107">Properties</span></span>

| <span data-ttu-id="f871b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f871b-108">Property</span></span> | <span data-ttu-id="f871b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f871b-109">Type</span></span>  | <span data-ttu-id="f871b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f871b-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="f871b-111">id</span><span class="sxs-lookup"><span data-stu-id="f871b-111">id</span></span>  | <span data-ttu-id="f871b-112">string</span><span class="sxs-lookup"><span data-stu-id="f871b-112">string</span></span> | <span data-ttu-id="f871b-113">Die ID der Arbeitsmappensitzung.</span><span class="sxs-lookup"><span data-stu-id="f871b-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="f871b-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="f871b-114">persistChanges</span></span> | <span data-ttu-id="f871b-115">string</span><span class="sxs-lookup"><span data-stu-id="f871b-115">string</span></span> |  <span data-ttu-id="f871b-116">`true` für eine beständige Sitzung</span><span class="sxs-lookup"><span data-stu-id="f871b-116">`true` for persistent session.</span></span> <span data-ttu-id="f871b-117">`false` für eine nicht-beständige Sitzung (Ansichtsmodus)</span><span class="sxs-lookup"><span data-stu-id="f871b-117">`false` for non-persistent session (view mode)</span></span> |

