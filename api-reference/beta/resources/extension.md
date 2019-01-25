---
title: extension-Ressourcentyp
description: Ein abstrakter Typ für die Unterstützung des offenen Typs openTypeExtension von OData v4.
localization_priority: Normal
ms.openlocfilehash: b261ceeff4639b8a602edbb411b34ab19d46ea8e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512745"
---
# <a name="extension-resource-type"></a><span data-ttu-id="7220b-103">extension-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7220b-103">extension resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7220b-104">Ein abstrakter Typ für die Unterstützung des offenen Typs [openTypeExtension](opentypeextension.md) von OData v4.</span><span class="sxs-lookup"><span data-stu-id="7220b-104">An abstract type to support the OData v4 open type [openTypeExtension](opentypeextension.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="7220b-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7220b-105">JSON representation</span></span>

<span data-ttu-id="7220b-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7220b-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a><span data-ttu-id="7220b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7220b-107">Properties</span></span>
| <span data-ttu-id="7220b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7220b-108">Property</span></span>     | <span data-ttu-id="7220b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="7220b-109">Type</span></span>   |<span data-ttu-id="7220b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7220b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7220b-111">id</span><span class="sxs-lookup"><span data-stu-id="7220b-111">id</span></span>|<span data-ttu-id="7220b-112">String</span><span class="sxs-lookup"><span data-stu-id="7220b-112">String</span></span>| <span data-ttu-id="7220b-113">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7220b-113">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7220b-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7220b-114">Relationships</span></span>
<span data-ttu-id="7220b-115">Keine</span><span class="sxs-lookup"><span data-stu-id="7220b-115">None</span></span>


## <a name="methods"></a><span data-ttu-id="7220b-116">Methoden</span><span class="sxs-lookup"><span data-stu-id="7220b-116">Methods</span></span>

<span data-ttu-id="7220b-117">Informationen zu tatsächlich unterstützten Methoden finden Sie in den Methoden des abgeleiteten Typs [openTypeExtension](opentypeextension.md).</span><span class="sxs-lookup"><span data-stu-id="7220b-117">See the methods of the derived type [openTypeExtension](opentypeextension.md) for actually supported methods.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/extension.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
