---
title: Ressourcentyp resourceReference
description: Komplexer Typ mit Eigenschaften des Insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 8cc7e686aebd531a25b6c1637fcf99338df09396
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572297"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="8dcac-103">Ressourcentyp resourceReference</span><span class="sxs-lookup"><span data-stu-id="8dcac-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dcac-104">Komplexer Typ mit Eigenschaften des [Insights](insights.md).</span><span class="sxs-lookup"><span data-stu-id="8dcac-104">Complex type containing properties of [insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="8dcac-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8dcac-105">JSON representation</span></span>

<span data-ttu-id="8dcac-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8dcac-106">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueLegacyExtendedProperty",
    "multiValueLegacyExtendedProperty"
  ],
  "@odata.type": "microsoft.graph.resourceReference"
}-->
```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="8dcac-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8dcac-107">Properties</span></span>

| <span data-ttu-id="8dcac-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8dcac-108">Property</span></span>      | <span data-ttu-id="8dcac-109">Typ</span><span class="sxs-lookup"><span data-stu-id="8dcac-109">Type</span></span>      | <span data-ttu-id="8dcac-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8dcac-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="8dcac-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="8dcac-111">webUrl</span></span>        | <span data-ttu-id="8dcac-112">String</span><span class="sxs-lookup"><span data-stu-id="8dcac-112">String</span></span>    | <span data-ttu-id="8dcac-113">Eine URL, die auf das verwiesene Element führende.</span><span class="sxs-lookup"><span data-stu-id="8dcac-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="8dcac-114">id</span><span class="sxs-lookup"><span data-stu-id="8dcac-114">id</span></span>            | <span data-ttu-id="8dcac-115">String</span><span class="sxs-lookup"><span data-stu-id="8dcac-115">String</span></span>    | <span data-ttu-id="8dcac-116">Eindeutiger Bezeichner des Elements.</span><span class="sxs-lookup"><span data-stu-id="8dcac-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="8dcac-117">type</span><span class="sxs-lookup"><span data-stu-id="8dcac-117">type</span></span>          | <span data-ttu-id="8dcac-118">String</span><span class="sxs-lookup"><span data-stu-id="8dcac-118">String</span></span>    | <span data-ttu-id="8dcac-119">Ein String-Wert, der verwendet werden kann, um das Element, wie beispielsweise "microsoft.graph.driveItem" klassifizieren</span><span class="sxs-lookup"><span data-stu-id="8dcac-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcereference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
