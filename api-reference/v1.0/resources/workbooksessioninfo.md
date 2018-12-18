---
title: workbookSessionInfo-Ressourcentyp
description: Enthält Informationen zu Arbeitsmappensitzungen.
author: lumine2008
ms.openlocfilehash: 1e097cad70a6058aab28ad85d7cf6b3c3b52ac75
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305985"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="34ed7-103">workbookSessionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="34ed7-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="34ed7-104">Enthält Informationen zu Arbeitsmappensitzungen.</span><span class="sxs-lookup"><span data-stu-id="34ed7-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="34ed7-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="34ed7-105">JSON representation</span></span>

<span data-ttu-id="34ed7-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="34ed7-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="34ed7-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="34ed7-107">Properties</span></span>

| <span data-ttu-id="34ed7-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="34ed7-108">Property</span></span> | <span data-ttu-id="34ed7-109">Typ</span><span class="sxs-lookup"><span data-stu-id="34ed7-109">Type</span></span>  | <span data-ttu-id="34ed7-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34ed7-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="34ed7-111">id</span><span class="sxs-lookup"><span data-stu-id="34ed7-111">id</span></span>  | <span data-ttu-id="34ed7-112">string</span><span class="sxs-lookup"><span data-stu-id="34ed7-112">string</span></span> | <span data-ttu-id="34ed7-113">Die ID der Arbeitsmappensitzung.</span><span class="sxs-lookup"><span data-stu-id="34ed7-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="34ed7-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="34ed7-114">persistChanges</span></span> | <span data-ttu-id="34ed7-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="34ed7-115">boolean</span></span> |  <span data-ttu-id="34ed7-116">`true` für eine beständige Sitzung</span><span class="sxs-lookup"><span data-stu-id="34ed7-116">`true` for persistent session.</span></span> <span data-ttu-id="34ed7-117">`false` für eine nicht-beständige Sitzung (Ansichtsmodus)</span><span class="sxs-lookup"><span data-stu-id="34ed7-117">`false` for non-persistent session (view mode)</span></span> |

