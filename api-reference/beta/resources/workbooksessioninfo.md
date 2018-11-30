---
title: workbookSessionInfo-Ressourcentyp
description: Enthält Informationen zu Arbeitsmappensitzungen.
ms.openlocfilehash: c04afe17c10edd8b136465d6d7ae3dbedb6307ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061494"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="bba91-103">workbookSessionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bba91-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="bba91-104">Enthält Informationen zu Arbeitsmappensitzungen.</span><span class="sxs-lookup"><span data-stu-id="bba91-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="bba91-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bba91-105">JSON representation</span></span>

<span data-ttu-id="bba91-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bba91-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="bba91-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bba91-107">Properties</span></span>

| <span data-ttu-id="bba91-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bba91-108">Property</span></span> | <span data-ttu-id="bba91-109">Typ</span><span class="sxs-lookup"><span data-stu-id="bba91-109">Type</span></span>  | <span data-ttu-id="bba91-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bba91-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="bba91-111">id</span><span class="sxs-lookup"><span data-stu-id="bba91-111">id</span></span>  | <span data-ttu-id="bba91-112">string</span><span class="sxs-lookup"><span data-stu-id="bba91-112">string</span></span> | <span data-ttu-id="bba91-113">Die ID der Arbeitsmappensitzung.</span><span class="sxs-lookup"><span data-stu-id="bba91-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="bba91-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="bba91-114">persistChanges</span></span> | <span data-ttu-id="bba91-115">string</span><span class="sxs-lookup"><span data-stu-id="bba91-115">string</span></span> |  <span data-ttu-id="bba91-116">`true` für eine beständige Sitzung</span><span class="sxs-lookup"><span data-stu-id="bba91-116">`true` for persistent session.</span></span> <span data-ttu-id="bba91-117">`false` für eine nicht-beständige Sitzung (Ansichtsmodus)</span><span class="sxs-lookup"><span data-stu-id="bba91-117">`false` for non-persistent session (view mode)</span></span> |

