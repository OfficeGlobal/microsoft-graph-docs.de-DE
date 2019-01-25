---
title: Ressourcentyp imageInfo
description: Einen komplexen Typ für die **Zuweisung** -Eigenschaft im VisualInfo Teil des Aktivität-Objekts darstellt.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 112b1dc3d1db45f3fe470c1c21d483b09c00202c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514915"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="97f74-103">Ressourcentyp imageInfo</span><span class="sxs-lookup"><span data-stu-id="97f74-103">imageInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97f74-104">Einen komplexen Typ für die **Zuweisung** -Eigenschaft im [VisualInfo](../resources/projectrome-visualinfo.md) Teil des [Aktivität](../resources/projectrome-activity.md) -Objekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="97f74-104">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="97f74-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="97f74-105">Properties</span></span>

|<span data-ttu-id="97f74-106">Name</span><span class="sxs-lookup"><span data-stu-id="97f74-106">Name</span></span> | <span data-ttu-id="97f74-107">Typ</span><span class="sxs-lookup"><span data-stu-id="97f74-107">Type</span></span> | <span data-ttu-id="97f74-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97f74-108">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="97f74-109">IconUrl</span><span class="sxs-lookup"><span data-stu-id="97f74-109">iconUrl</span></span> | <span data-ttu-id="97f74-110">String</span><span class="sxs-lookup"><span data-stu-id="97f74-110">String</span></span> | <span data-ttu-id="97f74-111">Optional; URI, der auf ein Symbol, die die Anwendung verwendet verweist, um die Aktivität generieren darstellt.</span><span class="sxs-lookup"><span data-stu-id="97f74-111">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="97f74-112">alternateText</span><span class="sxs-lookup"><span data-stu-id="97f74-112">alternateText</span></span> | <span data-ttu-id="97f74-113">String</span><span class="sxs-lookup"><span data-stu-id="97f74-113">String</span></span> | <span data-ttu-id="97f74-114">Optional; ALT-Text zugegriffen werden Inhalte für das Bild</span><span class="sxs-lookup"><span data-stu-id="97f74-114">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="97f74-115">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="97f74-115">addImageQuery</span></span> | <span data-ttu-id="97f74-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="97f74-116">Boolean</span></span> | <span data-ttu-id="97f74-117">Optional; Parameter verwendet, um den Server anzugeben kann dynamisch als Reaktion auf Parametrisierung Bild zu rendern.</span><span class="sxs-lookup"><span data-stu-id="97f74-117">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="97f74-118">Beispiel – ein hoher Kontrast-Bild</span><span class="sxs-lookup"><span data-stu-id="97f74-118">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97f74-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="97f74-119">JSON Representation</span></span>

<span data-ttu-id="97f74-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="97f74-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/projectrome-imageinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
