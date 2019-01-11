---
title: Ressourcentyp imageInfo
description: Einen komplexen Typ für die **Zuweisung** -Eigenschaft im VisualInfo Teil des Aktivität-Objekts darstellt.
localization_priority: Normal
ms.openlocfilehash: 2bac97ff945c0e0975ffa19636a954308b895e88
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856462"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="d5755-103">Ressourcentyp imageInfo</span><span class="sxs-lookup"><span data-stu-id="d5755-103">imageInfo resource type</span></span>

<span data-ttu-id="d5755-104">Einen komplexen Typ für die **Zuweisung** -Eigenschaft im [VisualInfo](../resources/projectrome-visualinfo.md) Teil des [Aktivität](../resources/projectrome-activity.md) -Objekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="d5755-104">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="d5755-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d5755-105">Properties</span></span>

|<span data-ttu-id="d5755-106">Name</span><span class="sxs-lookup"><span data-stu-id="d5755-106">Name</span></span> | <span data-ttu-id="d5755-107">Typ</span><span class="sxs-lookup"><span data-stu-id="d5755-107">Type</span></span> | <span data-ttu-id="d5755-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d5755-108">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="d5755-109">iconUrl</span><span class="sxs-lookup"><span data-stu-id="d5755-109">iconUrl</span></span> | <span data-ttu-id="d5755-110">String</span><span class="sxs-lookup"><span data-stu-id="d5755-110">String</span></span> | <span data-ttu-id="d5755-111">Optional; URI, der auf ein Symbol, die die Anwendung verwendet verweist, um die Aktivität generieren darstellt.</span><span class="sxs-lookup"><span data-stu-id="d5755-111">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="d5755-112">alternateText</span><span class="sxs-lookup"><span data-stu-id="d5755-112">alternateText</span></span> | <span data-ttu-id="d5755-113">String</span><span class="sxs-lookup"><span data-stu-id="d5755-113">String</span></span> | <span data-ttu-id="d5755-114">Optional; ALT-Text zugegriffen werden Inhalte für das Bild</span><span class="sxs-lookup"><span data-stu-id="d5755-114">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="d5755-115">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="d5755-115">addImageQuery</span></span> | <span data-ttu-id="d5755-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5755-116">Boolean</span></span> | <span data-ttu-id="d5755-117">Optional; Parameter verwendet, um den Server anzugeben kann dynamisch als Reaktion auf Parametrisierung Bild zu rendern.</span><span class="sxs-lookup"><span data-stu-id="d5755-117">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="d5755-118">Beispiel – ein hoher Kontrast-Bild</span><span class="sxs-lookup"><span data-stu-id="d5755-118">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d5755-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d5755-119">JSON Representation</span></span>

<span data-ttu-id="d5755-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d5755-120">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
