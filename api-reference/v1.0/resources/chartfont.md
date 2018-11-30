---
title: ChartFont-Ressourcentyp
description: Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Diagrammobjekt dar.
ms.openlocfilehash: dc4b1f8cd0653d89c3486a61604dd09c0e23cb2c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017168"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="23c09-103">ChartFont-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="23c09-103">ChartFont resource type</span></span>

<span data-ttu-id="23c09-104">Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Diagrammobjekt dar.</span><span class="sxs-lookup"><span data-stu-id="23c09-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="23c09-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="23c09-105">Methods</span></span>

| <span data-ttu-id="23c09-106">Methode</span><span class="sxs-lookup"><span data-stu-id="23c09-106">Method</span></span>           | <span data-ttu-id="23c09-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="23c09-107">Return Type</span></span>    |<span data-ttu-id="23c09-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23c09-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="23c09-109">ChartFont abrufen</span><span class="sxs-lookup"><span data-stu-id="23c09-109">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="23c09-110">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="23c09-110">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="23c09-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chartFont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="23c09-111">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="23c09-112">Update</span><span class="sxs-lookup"><span data-stu-id="23c09-112">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="23c09-113">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="23c09-113">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="23c09-114">Dient zum Aktualisieren des ChartFont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="23c09-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="23c09-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="23c09-115">Properties</span></span>
| <span data-ttu-id="23c09-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23c09-116">Property</span></span>     | <span data-ttu-id="23c09-117">Typ</span><span class="sxs-lookup"><span data-stu-id="23c09-117">Type</span></span>   |<span data-ttu-id="23c09-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23c09-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23c09-119">bold</span><span class="sxs-lookup"><span data-stu-id="23c09-119">bold</span></span>|<span data-ttu-id="23c09-120">boolean</span><span class="sxs-lookup"><span data-stu-id="23c09-120">boolean</span></span>|<span data-ttu-id="23c09-121">Stellt den Fett-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="23c09-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="23c09-122">color</span><span class="sxs-lookup"><span data-stu-id="23c09-122">color</span></span>|<span data-ttu-id="23c09-123">string</span><span class="sxs-lookup"><span data-stu-id="23c09-123">string</span></span>|<span data-ttu-id="23c09-p101">HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.</span><span class="sxs-lookup"><span data-stu-id="23c09-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="23c09-127">italic</span><span class="sxs-lookup"><span data-stu-id="23c09-127">italic</span></span>|<span data-ttu-id="23c09-128">boolean</span><span class="sxs-lookup"><span data-stu-id="23c09-128">boolean</span></span>|<span data-ttu-id="23c09-129">Stellt den Kursiv-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="23c09-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="23c09-130">name</span><span class="sxs-lookup"><span data-stu-id="23c09-130">name</span></span>|<span data-ttu-id="23c09-131">string</span><span class="sxs-lookup"><span data-stu-id="23c09-131">string</span></span>|<span data-ttu-id="23c09-132">Schriftartname (z. B. "Calibri")</span><span class="sxs-lookup"><span data-stu-id="23c09-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="23c09-133">size</span><span class="sxs-lookup"><span data-stu-id="23c09-133">size</span></span>|<span data-ttu-id="23c09-134">double</span><span class="sxs-lookup"><span data-stu-id="23c09-134">double</span></span>|<span data-ttu-id="23c09-135">Der Schriftgrad (z. B. 11)</span><span class="sxs-lookup"><span data-stu-id="23c09-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="23c09-136">underline</span><span class="sxs-lookup"><span data-stu-id="23c09-136">underline</span></span>|<span data-ttu-id="23c09-137">string</span><span class="sxs-lookup"><span data-stu-id="23c09-137">string</span></span>|<span data-ttu-id="23c09-138">Typ der Unterstreichung auf die Schriftart.</span><span class="sxs-lookup"><span data-stu-id="23c09-138">Type of underline applied to the font.</span></span> <span data-ttu-id="23c09-139">Die möglichen Werte sind: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="23c09-139">The possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23c09-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="23c09-140">Relationships</span></span>
<span data-ttu-id="23c09-141">Keine</span><span class="sxs-lookup"><span data-stu-id="23c09-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="23c09-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="23c09-142">JSON representation</span></span>

<span data-ttu-id="23c09-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="23c09-143">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartFont"
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
<!-- {
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->