---
title: RangeFont-Ressourcentyp
description: Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Objekt dar.
ms.openlocfilehash: bafb7c052458c7b3f4001d7e999acc14c7aaabee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018947"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="0abfa-103">RangeFont-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0abfa-103">RangeFont resource type</span></span>

<span data-ttu-id="0abfa-104">Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Objekt dar.</span><span class="sxs-lookup"><span data-stu-id="0abfa-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="0abfa-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="0abfa-105">Methods</span></span>

| <span data-ttu-id="0abfa-106">Methode</span><span class="sxs-lookup"><span data-stu-id="0abfa-106">Method</span></span>           | <span data-ttu-id="0abfa-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0abfa-107">Return Type</span></span>    |<span data-ttu-id="0abfa-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0abfa-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0abfa-109">RangeFont abrufen</span><span class="sxs-lookup"><span data-stu-id="0abfa-109">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="0abfa-110">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="0abfa-110">WorkbookRangeFont</span></span>](rangefont.md) |<span data-ttu-id="0abfa-111">Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0abfa-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="0abfa-112">Update</span><span class="sxs-lookup"><span data-stu-id="0abfa-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="0abfa-113">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="0abfa-113">WorkbookRangeFont</span></span>](rangefont.md)   |<span data-ttu-id="0abfa-114">Dient zum Aktualisieren des RangeFont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0abfa-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0abfa-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0abfa-115">Properties</span></span>
| <span data-ttu-id="0abfa-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0abfa-116">Property</span></span>     | <span data-ttu-id="0abfa-117">Typ</span><span class="sxs-lookup"><span data-stu-id="0abfa-117">Type</span></span>   |<span data-ttu-id="0abfa-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0abfa-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0abfa-119">bold</span><span class="sxs-lookup"><span data-stu-id="0abfa-119">bold</span></span>|<span data-ttu-id="0abfa-120">boolean</span><span class="sxs-lookup"><span data-stu-id="0abfa-120">boolean</span></span>|<span data-ttu-id="0abfa-121">Stellt den Fett-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="0abfa-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="0abfa-122">color</span><span class="sxs-lookup"><span data-stu-id="0abfa-122">color</span></span>|<span data-ttu-id="0abfa-123">string</span><span class="sxs-lookup"><span data-stu-id="0abfa-123">string</span></span>|<span data-ttu-id="0abfa-p101">HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.</span><span class="sxs-lookup"><span data-stu-id="0abfa-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="0abfa-127">italic</span><span class="sxs-lookup"><span data-stu-id="0abfa-127">italic</span></span>|<span data-ttu-id="0abfa-128">boolean</span><span class="sxs-lookup"><span data-stu-id="0abfa-128">boolean</span></span>|<span data-ttu-id="0abfa-129">Stellt den Kursiv-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="0abfa-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="0abfa-130">name</span><span class="sxs-lookup"><span data-stu-id="0abfa-130">name</span></span>|<span data-ttu-id="0abfa-131">string</span><span class="sxs-lookup"><span data-stu-id="0abfa-131">string</span></span>|<span data-ttu-id="0abfa-132">Schriftartname (z. B. "Calibri")</span><span class="sxs-lookup"><span data-stu-id="0abfa-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="0abfa-133">size</span><span class="sxs-lookup"><span data-stu-id="0abfa-133">size</span></span>|<span data-ttu-id="0abfa-134">double</span><span class="sxs-lookup"><span data-stu-id="0abfa-134">double</span></span>|<span data-ttu-id="0abfa-135">Schriftgrad</span><span class="sxs-lookup"><span data-stu-id="0abfa-135">Font size.</span></span>|
|<span data-ttu-id="0abfa-136">underline</span><span class="sxs-lookup"><span data-stu-id="0abfa-136">underline</span></span>|<span data-ttu-id="0abfa-137">string</span><span class="sxs-lookup"><span data-stu-id="0abfa-137">string</span></span>|<span data-ttu-id="0abfa-138">Typ der Unterstreichung auf die Schriftart.</span><span class="sxs-lookup"><span data-stu-id="0abfa-138">Type of underline applied to the font.</span></span> <span data-ttu-id="0abfa-139">Die möglichen Werte sind: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="0abfa-139">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0abfa-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0abfa-140">Relationships</span></span>
<span data-ttu-id="0abfa-141">Keine</span><span class="sxs-lookup"><span data-stu-id="0abfa-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0abfa-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0abfa-142">JSON representation</span></span>

<span data-ttu-id="0abfa-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0abfa-143">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFont"
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
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->