---
title: ChartFont-Ressourcentyp
description: Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Diagrammobjekt dar.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: c507a966dc6b29e46935c5c77a85b557a84cc69c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518324"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="ef808-103">ChartFont-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ef808-103">ChartFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef808-104">Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Diagrammobjekt dar.</span><span class="sxs-lookup"><span data-stu-id="ef808-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="ef808-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="ef808-105">Methods</span></span>

| <span data-ttu-id="ef808-106">Methode</span><span class="sxs-lookup"><span data-stu-id="ef808-106">Method</span></span>           | <span data-ttu-id="ef808-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ef808-107">Return Type</span></span>    |<span data-ttu-id="ef808-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ef808-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef808-109">ChartFont abrufen</span><span class="sxs-lookup"><span data-stu-id="ef808-109">[Get ChartFont](../api/chartfont-get.md)</span></span> | <span data-ttu-id="ef808-110">ChartFont</span><span class="sxs-lookup"><span data-stu-id="ef808-110">[ChartFont](chartfont.md)</span></span> |<span data-ttu-id="ef808-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chartFont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ef808-111">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="ef808-112">Update</span><span class="sxs-lookup"><span data-stu-id="ef808-112">Update</span></span>](../api/chartfont-update.md) | <span data-ttu-id="ef808-113">ChartFont</span><span class="sxs-lookup"><span data-stu-id="ef808-113">[ChartFont](chartfont.md)</span></span>   |<span data-ttu-id="ef808-114">Dient zum Aktualisieren des ChartFont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ef808-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ef808-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ef808-115">Properties</span></span>
| <span data-ttu-id="ef808-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ef808-116">Property</span></span>     | <span data-ttu-id="ef808-117">Typ</span><span class="sxs-lookup"><span data-stu-id="ef808-117">Type</span></span>   |<span data-ttu-id="ef808-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ef808-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef808-119">bold</span><span class="sxs-lookup"><span data-stu-id="ef808-119">bold</span></span>|<span data-ttu-id="ef808-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ef808-120">boolean</span></span>|<span data-ttu-id="ef808-121">Stellt den Fett-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="ef808-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="ef808-122">color</span><span class="sxs-lookup"><span data-stu-id="ef808-122">color</span></span>|<span data-ttu-id="ef808-123">string</span><span class="sxs-lookup"><span data-stu-id="ef808-123">string</span></span>|<span data-ttu-id="ef808-p101">HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.</span><span class="sxs-lookup"><span data-stu-id="ef808-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="ef808-127">italic</span><span class="sxs-lookup"><span data-stu-id="ef808-127">italic</span></span>|<span data-ttu-id="ef808-128">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ef808-128">boolean</span></span>|<span data-ttu-id="ef808-129">Stellt den Kursiv-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="ef808-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="ef808-130">name</span><span class="sxs-lookup"><span data-stu-id="ef808-130">name</span></span>|<span data-ttu-id="ef808-131">string</span><span class="sxs-lookup"><span data-stu-id="ef808-131">string</span></span>|<span data-ttu-id="ef808-132">Schriftartname (z. B. "Calibri")</span><span class="sxs-lookup"><span data-stu-id="ef808-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="ef808-133">size</span><span class="sxs-lookup"><span data-stu-id="ef808-133">size</span></span>|<span data-ttu-id="ef808-134">double</span><span class="sxs-lookup"><span data-stu-id="ef808-134">double</span></span>|<span data-ttu-id="ef808-135">Der Schriftgrad (z. B. 11)</span><span class="sxs-lookup"><span data-stu-id="ef808-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="ef808-136">underline</span><span class="sxs-lookup"><span data-stu-id="ef808-136">underline</span></span>|<span data-ttu-id="ef808-137">string</span><span class="sxs-lookup"><span data-stu-id="ef808-137">string</span></span>|<span data-ttu-id="ef808-p102">Art der auf die Schriftart angewendeten Unterstreichung. Mögliche Werte: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="ef808-p102">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef808-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ef808-140">Relationships</span></span>
<span data-ttu-id="ef808-141">Keine</span><span class="sxs-lookup"><span data-stu-id="ef808-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ef808-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ef808-142">JSON representation</span></span>

<span data-ttu-id="ef808-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ef808-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartFont"
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
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartfont.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
