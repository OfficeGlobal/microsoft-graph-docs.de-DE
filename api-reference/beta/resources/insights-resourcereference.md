---
title: Ressourcentyp resourceReference
description: Komplexer Typ mit Eigenschaften des Insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4fa4563904472fad9fc28fa4acb10b77887b5872
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520004"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="d66e8-103">Ressourcentyp resourceReference</span><span class="sxs-lookup"><span data-stu-id="d66e8-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d66e8-104">Komplexer Typ mit Eigenschaften des [Insights](insights.md).</span><span class="sxs-lookup"><span data-stu-id="d66e8-104">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d66e8-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d66e8-105">JSON representation</span></span>

<span data-ttu-id="d66e8-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d66e8-106">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="d66e8-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d66e8-107">Properties</span></span>

| <span data-ttu-id="d66e8-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d66e8-108">Property</span></span>      | <span data-ttu-id="d66e8-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d66e8-109">Type</span></span>      | <span data-ttu-id="d66e8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d66e8-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="d66e8-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="d66e8-111">webUrl</span></span>        | <span data-ttu-id="d66e8-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d66e8-112">String</span></span>    | <span data-ttu-id="d66e8-113">Eine URL, die auf das verwiesene Element führende.</span><span class="sxs-lookup"><span data-stu-id="d66e8-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="d66e8-114">id</span><span class="sxs-lookup"><span data-stu-id="d66e8-114">id</span></span>            | <span data-ttu-id="d66e8-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d66e8-115">String</span></span>    | <span data-ttu-id="d66e8-116">Eindeutiger Bezeichner des Elements.</span><span class="sxs-lookup"><span data-stu-id="d66e8-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="d66e8-117">type</span><span class="sxs-lookup"><span data-stu-id="d66e8-117">type</span></span>          | <span data-ttu-id="d66e8-118">String</span><span class="sxs-lookup"><span data-stu-id="d66e8-118">String</span></span>    | <span data-ttu-id="d66e8-119">Ein String-Wert, der verwendet werden kann, um das Element, wie beispielsweise "microsoft.graph.driveItem" klassifizieren</span><span class="sxs-lookup"><span data-stu-id="d66e8-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcereference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
