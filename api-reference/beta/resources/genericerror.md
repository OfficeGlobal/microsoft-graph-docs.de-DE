---
title: Allgemeiner Fehler Ressourcentyp
description: Ein allgemeiner Fehler.
localization_priority: Normal
ms.openlocfilehash: d3c7e9cd7ff7be635adfbf329170068cd944f0b2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524128"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="b8cbe-103">Allgemeiner Fehler Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b8cbe-103">genericError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8cbe-104">Ein allgemeiner Fehler.</span><span class="sxs-lookup"><span data-stu-id="b8cbe-104">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="b8cbe-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b8cbe-105">Properties</span></span>

| <span data-ttu-id="b8cbe-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8cbe-106">Property</span></span> | <span data-ttu-id="b8cbe-107">Typ</span><span class="sxs-lookup"><span data-stu-id="b8cbe-107">Type</span></span> | <span data-ttu-id="b8cbe-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8cbe-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="b8cbe-109">message</span><span class="sxs-lookup"><span data-stu-id="b8cbe-109">message</span></span> | <span data-ttu-id="b8cbe-110">String</span><span class="sxs-lookup"><span data-stu-id="b8cbe-110">String</span></span> | <span data-ttu-id="b8cbe-111">Die Fehlermeldung.</span><span class="sxs-lookup"><span data-stu-id="b8cbe-111">The error message.</span></span> |
| <span data-ttu-id="b8cbe-112">code</span><span class="sxs-lookup"><span data-stu-id="b8cbe-112">code</span></span> | <span data-ttu-id="b8cbe-113">String</span><span class="sxs-lookup"><span data-stu-id="b8cbe-113">String</span></span> | <span data-ttu-id="b8cbe-114">Der Fehlercode.</span><span class="sxs-lookup"><span data-stu-id="b8cbe-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b8cbe-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b8cbe-115">JSON representation</span></span>

<span data-ttu-id="b8cbe-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b8cbe-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/genericerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
