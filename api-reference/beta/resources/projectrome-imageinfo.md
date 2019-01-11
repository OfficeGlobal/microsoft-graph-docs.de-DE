---
title: Ressourcentyp imageInfo
description: Einen komplexen Typ für die **Zuweisung** -Eigenschaft im VisualInfo Teil des Aktivität-Objekts darstellt.
localization_priority: Normal
ms.openlocfilehash: 9df93e24c2019f246fc9da269b40ab690ae81aa4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828567"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="c7350-103">Ressourcentyp imageInfo</span><span class="sxs-lookup"><span data-stu-id="c7350-103">imageInfo resource type</span></span>

> <span data-ttu-id="c7350-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c7350-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7350-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c7350-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c7350-106">Einen komplexen Typ für die **Zuweisung** -Eigenschaft im [VisualInfo](../resources/projectrome-visualinfo.md) Teil des [Aktivität](../resources/projectrome-activity.md) -Objekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="c7350-106">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="c7350-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c7350-107">Properties</span></span>

|<span data-ttu-id="c7350-108">Name</span><span class="sxs-lookup"><span data-stu-id="c7350-108">Name</span></span> | <span data-ttu-id="c7350-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c7350-109">Type</span></span> | <span data-ttu-id="c7350-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7350-110">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="c7350-111">iconUrl</span><span class="sxs-lookup"><span data-stu-id="c7350-111">iconUrl</span></span> | <span data-ttu-id="c7350-112">String</span><span class="sxs-lookup"><span data-stu-id="c7350-112">String</span></span> | <span data-ttu-id="c7350-113">Optional; URI, der auf ein Symbol, die die Anwendung verwendet verweist, um die Aktivität generieren darstellt.</span><span class="sxs-lookup"><span data-stu-id="c7350-113">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="c7350-114">alternateText</span><span class="sxs-lookup"><span data-stu-id="c7350-114">alternateText</span></span> | <span data-ttu-id="c7350-115">String</span><span class="sxs-lookup"><span data-stu-id="c7350-115">String</span></span> | <span data-ttu-id="c7350-116">Optional; ALT-Text zugegriffen werden Inhalte für das Bild</span><span class="sxs-lookup"><span data-stu-id="c7350-116">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="c7350-117">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="c7350-117">addImageQuery</span></span> | <span data-ttu-id="c7350-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c7350-118">Boolean</span></span> | <span data-ttu-id="c7350-119">Optional; Parameter verwendet, um den Server anzugeben kann dynamisch als Reaktion auf Parametrisierung Bild zu rendern.</span><span class="sxs-lookup"><span data-stu-id="c7350-119">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="c7350-120">Beispiel – ein hoher Kontrast-Bild</span><span class="sxs-lookup"><span data-stu-id="c7350-120">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7350-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c7350-121">JSON Representation</span></span>

<span data-ttu-id="c7350-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c7350-122">Here is a JSON representation of the resource</span></span>

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
