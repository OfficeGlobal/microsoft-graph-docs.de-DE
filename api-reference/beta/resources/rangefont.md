---
title: RangeFont-Ressourcentyp
description: Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Objekt dar.
ms.openlocfilehash: fc1f3e35bb2ea612dd462d97075ad9757e27bf22
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058788"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="f23ed-103">RangeFont-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f23ed-103">RangeFont resource type</span></span>

> <span data-ttu-id="f23ed-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f23ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f23ed-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f23ed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f23ed-106">Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Objekt dar.</span><span class="sxs-lookup"><span data-stu-id="f23ed-106">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="f23ed-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="f23ed-107">Methods</span></span>

| <span data-ttu-id="f23ed-108">Methode</span><span class="sxs-lookup"><span data-stu-id="f23ed-108">Method</span></span>           | <span data-ttu-id="f23ed-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f23ed-109">Return Type</span></span>    |<span data-ttu-id="f23ed-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f23ed-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f23ed-111">RangeFont abrufen</span><span class="sxs-lookup"><span data-stu-id="f23ed-111">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="f23ed-112">RangeFont</span><span class="sxs-lookup"><span data-stu-id="f23ed-112">RangeFont</span></span>](rangefont.md) |<span data-ttu-id="f23ed-113">Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f23ed-113">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="f23ed-114">Update</span><span class="sxs-lookup"><span data-stu-id="f23ed-114">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="f23ed-115">RangeFont</span><span class="sxs-lookup"><span data-stu-id="f23ed-115">RangeFont</span></span>](rangefont.md)   |<span data-ttu-id="f23ed-116">Dient zum Aktualisieren des RangeFont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f23ed-116">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f23ed-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f23ed-117">Properties</span></span>
| <span data-ttu-id="f23ed-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f23ed-118">Property</span></span>     | <span data-ttu-id="f23ed-119">Typ</span><span class="sxs-lookup"><span data-stu-id="f23ed-119">Type</span></span>   |<span data-ttu-id="f23ed-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f23ed-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f23ed-121">bold</span><span class="sxs-lookup"><span data-stu-id="f23ed-121">bold</span></span>|<span data-ttu-id="f23ed-122">boolean</span><span class="sxs-lookup"><span data-stu-id="f23ed-122">boolean</span></span>|<span data-ttu-id="f23ed-123">Stellt den Fett-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="f23ed-123">Represents the bold status of font.</span></span>|
|<span data-ttu-id="f23ed-124">color</span><span class="sxs-lookup"><span data-stu-id="f23ed-124">color</span></span>|<span data-ttu-id="f23ed-125">string</span><span class="sxs-lookup"><span data-stu-id="f23ed-125">string</span></span>|<span data-ttu-id="f23ed-p102">HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.</span><span class="sxs-lookup"><span data-stu-id="f23ed-p102">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="f23ed-129">italic</span><span class="sxs-lookup"><span data-stu-id="f23ed-129">italic</span></span>|<span data-ttu-id="f23ed-130">boolean</span><span class="sxs-lookup"><span data-stu-id="f23ed-130">boolean</span></span>|<span data-ttu-id="f23ed-131">Stellt den Kursiv-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="f23ed-131">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="f23ed-132">name</span><span class="sxs-lookup"><span data-stu-id="f23ed-132">name</span></span>|<span data-ttu-id="f23ed-133">string</span><span class="sxs-lookup"><span data-stu-id="f23ed-133">string</span></span>|<span data-ttu-id="f23ed-134">Schriftartname (z. B. "Calibri")</span><span class="sxs-lookup"><span data-stu-id="f23ed-134">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="f23ed-135">size</span><span class="sxs-lookup"><span data-stu-id="f23ed-135">size</span></span>|<span data-ttu-id="f23ed-136">double</span><span class="sxs-lookup"><span data-stu-id="f23ed-136">double</span></span>|<span data-ttu-id="f23ed-137">Schriftgrad</span><span class="sxs-lookup"><span data-stu-id="f23ed-137">Font size.</span></span>|
|<span data-ttu-id="f23ed-138">underline</span><span class="sxs-lookup"><span data-stu-id="f23ed-138">underline</span></span>|<span data-ttu-id="f23ed-139">string</span><span class="sxs-lookup"><span data-stu-id="f23ed-139">string</span></span>|<span data-ttu-id="f23ed-p103">Art der auf die Schriftart angewendete Unterstreichung. Die folgenden Werte sind möglich: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="f23ed-p103">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f23ed-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f23ed-142">Relationships</span></span>
<span data-ttu-id="f23ed-143">Keine</span><span class="sxs-lookup"><span data-stu-id="f23ed-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f23ed-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f23ed-144">JSON representation</span></span>

<span data-ttu-id="f23ed-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f23ed-145">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->