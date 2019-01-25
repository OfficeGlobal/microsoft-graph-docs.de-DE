---
title: RangeFont-Ressourcentyp
description: Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Objekt dar.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 2dee07b7d2573081650bdd15799e4884c774e171
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507964"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="69835-103">RangeFont-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="69835-103">RangeFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69835-104">Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Objekt dar.</span><span class="sxs-lookup"><span data-stu-id="69835-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="69835-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="69835-105">Methods</span></span>

| <span data-ttu-id="69835-106">Methode</span><span class="sxs-lookup"><span data-stu-id="69835-106">Method</span></span>           | <span data-ttu-id="69835-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="69835-107">Return Type</span></span>    |<span data-ttu-id="69835-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69835-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69835-109">RangeFont abrufen</span><span class="sxs-lookup"><span data-stu-id="69835-109">[Get RangeFont](../api/rangefont-get.md)</span></span> | <span data-ttu-id="69835-110">RangeFont</span><span class="sxs-lookup"><span data-stu-id="69835-110">[RangeFont](rangefont.md)</span></span> |<span data-ttu-id="69835-111">Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="69835-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="69835-112">Update</span><span class="sxs-lookup"><span data-stu-id="69835-112">Update</span></span>](../api/rangefont-update.md) | <span data-ttu-id="69835-113">RangeFont</span><span class="sxs-lookup"><span data-stu-id="69835-113">[RangeFont](rangefont.md)</span></span>   |<span data-ttu-id="69835-114">Dient zum Aktualisieren des RangeFont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="69835-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="69835-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="69835-115">Properties</span></span>
| <span data-ttu-id="69835-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="69835-116">Property</span></span>     | <span data-ttu-id="69835-117">Typ</span><span class="sxs-lookup"><span data-stu-id="69835-117">Type</span></span>   |<span data-ttu-id="69835-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69835-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69835-119">bold</span><span class="sxs-lookup"><span data-stu-id="69835-119">bold</span></span>|<span data-ttu-id="69835-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="69835-120">boolean</span></span>|<span data-ttu-id="69835-121">Stellt den Fett-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="69835-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="69835-122">color</span><span class="sxs-lookup"><span data-stu-id="69835-122">color</span></span>|<span data-ttu-id="69835-123">string</span><span class="sxs-lookup"><span data-stu-id="69835-123">string</span></span>|<span data-ttu-id="69835-p101">HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.</span><span class="sxs-lookup"><span data-stu-id="69835-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="69835-127">italic</span><span class="sxs-lookup"><span data-stu-id="69835-127">italic</span></span>|<span data-ttu-id="69835-128">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="69835-128">boolean</span></span>|<span data-ttu-id="69835-129">Stellt den Kursiv-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="69835-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="69835-130">name</span><span class="sxs-lookup"><span data-stu-id="69835-130">name</span></span>|<span data-ttu-id="69835-131">string</span><span class="sxs-lookup"><span data-stu-id="69835-131">string</span></span>|<span data-ttu-id="69835-132">Schriftartname (z. B. "Calibri")</span><span class="sxs-lookup"><span data-stu-id="69835-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="69835-133">size</span><span class="sxs-lookup"><span data-stu-id="69835-133">size</span></span>|<span data-ttu-id="69835-134">double</span><span class="sxs-lookup"><span data-stu-id="69835-134">double</span></span>|<span data-ttu-id="69835-135">Schriftgrad</span><span class="sxs-lookup"><span data-stu-id="69835-135">Font size.</span></span>|
|<span data-ttu-id="69835-136">underline</span><span class="sxs-lookup"><span data-stu-id="69835-136">underline</span></span>|<span data-ttu-id="69835-137">string</span><span class="sxs-lookup"><span data-stu-id="69835-137">string</span></span>|<span data-ttu-id="69835-p102">Art der auf die Schriftart angewendete Unterstreichung. Die folgenden Werte sind möglich: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="69835-p102">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69835-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="69835-140">Relationships</span></span>
<span data-ttu-id="69835-141">Keine</span><span class="sxs-lookup"><span data-stu-id="69835-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="69835-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="69835-142">JSON representation</span></span>

<span data-ttu-id="69835-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="69835-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rangefont.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
