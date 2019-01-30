---
title: Ressourcentyp resourceReference
description: Komplexer Typ mit Eigenschaften des Insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4fa4563904472fad9fc28fa4acb10b77887b5872
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642758"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="efedd-103">Ressourcentyp resourceReference</span><span class="sxs-lookup"><span data-stu-id="efedd-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efedd-104">Komplexer Typ mit Eigenschaften des [Insights](insights.md).</span><span class="sxs-lookup"><span data-stu-id="efedd-104">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="efedd-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="efedd-105">JSON representation</span></span>

<span data-ttu-id="efedd-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="efedd-106">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="efedd-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="efedd-107">Properties</span></span>

| <span data-ttu-id="efedd-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="efedd-108">Property</span></span>      | <span data-ttu-id="efedd-109">Typ</span><span class="sxs-lookup"><span data-stu-id="efedd-109">Type</span></span>      | <span data-ttu-id="efedd-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="efedd-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="efedd-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="efedd-111">webUrl</span></span>        | <span data-ttu-id="efedd-112">String</span><span class="sxs-lookup"><span data-stu-id="efedd-112">String</span></span>    | <span data-ttu-id="efedd-113">Eine URL, die auf das verwiesene Element führende.</span><span class="sxs-lookup"><span data-stu-id="efedd-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="efedd-114">id</span><span class="sxs-lookup"><span data-stu-id="efedd-114">id</span></span>            | <span data-ttu-id="efedd-115">String</span><span class="sxs-lookup"><span data-stu-id="efedd-115">String</span></span>    | <span data-ttu-id="efedd-116">Eindeutiger Bezeichner des Elements.</span><span class="sxs-lookup"><span data-stu-id="efedd-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="efedd-117">type</span><span class="sxs-lookup"><span data-stu-id="efedd-117">type</span></span>          | <span data-ttu-id="efedd-118">String</span><span class="sxs-lookup"><span data-stu-id="efedd-118">String</span></span>    | <span data-ttu-id="efedd-119">Ein String-Wert, der verwendet werden kann, um das Element, wie beispielsweise "microsoft.graph.driveItem" klassifizieren</span><span class="sxs-lookup"><span data-stu-id="efedd-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcereference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
