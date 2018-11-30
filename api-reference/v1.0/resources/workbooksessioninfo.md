---
title: workbookSessionInfo-Ressourcentyp
description: Enthält Informationen zu Arbeitsmappensitzungen.
ms.openlocfilehash: 84d0306a7a25aaa29e4f1eb9b87708cc97d6b50f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017902"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="73431-103">workbookSessionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="73431-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="73431-104">Enthält Informationen zu Arbeitsmappensitzungen.</span><span class="sxs-lookup"><span data-stu-id="73431-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="73431-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="73431-105">JSON representation</span></span>

<span data-ttu-id="73431-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="73431-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="73431-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="73431-107">Properties</span></span>

| <span data-ttu-id="73431-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="73431-108">Property</span></span> | <span data-ttu-id="73431-109">Typ</span><span class="sxs-lookup"><span data-stu-id="73431-109">Type</span></span>  | <span data-ttu-id="73431-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73431-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="73431-111">id</span><span class="sxs-lookup"><span data-stu-id="73431-111">id</span></span>  | <span data-ttu-id="73431-112">string</span><span class="sxs-lookup"><span data-stu-id="73431-112">string</span></span> | <span data-ttu-id="73431-113">Die ID der Arbeitsmappensitzung.</span><span class="sxs-lookup"><span data-stu-id="73431-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="73431-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="73431-114">persistChanges</span></span> | <span data-ttu-id="73431-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="73431-115">boolean</span></span> |  <span data-ttu-id="73431-116">`true` für eine beständige Sitzung</span><span class="sxs-lookup"><span data-stu-id="73431-116">`true` for persistent session.</span></span> <span data-ttu-id="73431-117">`false` für eine nicht-beständige Sitzung (Ansichtsmodus)</span><span class="sxs-lookup"><span data-stu-id="73431-117">`false` for non-persistent session (view mode)</span></span> |

