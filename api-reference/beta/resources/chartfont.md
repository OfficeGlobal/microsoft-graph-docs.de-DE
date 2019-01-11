---
title: ChartFont-Ressourcentyp
description: Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Diagrammobjekt dar.
localization_priority: Normal
ms.openlocfilehash: 0df14f98993c33b6b3eb3c0b2ea9fbdf211a8124
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824164"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="16079-103">ChartFont-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="16079-103">ChartFont resource type</span></span>

> <span data-ttu-id="16079-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="16079-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16079-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16079-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16079-106">Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Diagrammobjekt dar.</span><span class="sxs-lookup"><span data-stu-id="16079-106">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="16079-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="16079-107">Methods</span></span>

| <span data-ttu-id="16079-108">Methode</span><span class="sxs-lookup"><span data-stu-id="16079-108">Method</span></span>           | <span data-ttu-id="16079-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="16079-109">Return Type</span></span>    |<span data-ttu-id="16079-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16079-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="16079-111">ChartFont abrufen</span><span class="sxs-lookup"><span data-stu-id="16079-111">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="16079-112">ChartFont</span><span class="sxs-lookup"><span data-stu-id="16079-112">ChartFont</span></span>](chartfont.md) |<span data-ttu-id="16079-113">Dient zum Lesen der Eigenschaften und der Beziehungen des chartFont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="16079-113">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="16079-114">Update</span><span class="sxs-lookup"><span data-stu-id="16079-114">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="16079-115">ChartFont</span><span class="sxs-lookup"><span data-stu-id="16079-115">ChartFont</span></span>](chartfont.md)   |<span data-ttu-id="16079-116">Dient zum Aktualisieren des ChartFont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="16079-116">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="16079-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="16079-117">Properties</span></span>
| <span data-ttu-id="16079-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="16079-118">Property</span></span>     | <span data-ttu-id="16079-119">Typ</span><span class="sxs-lookup"><span data-stu-id="16079-119">Type</span></span>   |<span data-ttu-id="16079-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16079-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16079-121">bold</span><span class="sxs-lookup"><span data-stu-id="16079-121">bold</span></span>|<span data-ttu-id="16079-122">boolean</span><span class="sxs-lookup"><span data-stu-id="16079-122">boolean</span></span>|<span data-ttu-id="16079-123">Stellt den Fett-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="16079-123">Represents the bold status of font.</span></span>|
|<span data-ttu-id="16079-124">color</span><span class="sxs-lookup"><span data-stu-id="16079-124">color</span></span>|<span data-ttu-id="16079-125">string</span><span class="sxs-lookup"><span data-stu-id="16079-125">string</span></span>|<span data-ttu-id="16079-p102">HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.</span><span class="sxs-lookup"><span data-stu-id="16079-p102">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="16079-129">italic</span><span class="sxs-lookup"><span data-stu-id="16079-129">italic</span></span>|<span data-ttu-id="16079-130">boolean</span><span class="sxs-lookup"><span data-stu-id="16079-130">boolean</span></span>|<span data-ttu-id="16079-131">Stellt den Kursiv-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="16079-131">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="16079-132">name</span><span class="sxs-lookup"><span data-stu-id="16079-132">name</span></span>|<span data-ttu-id="16079-133">string</span><span class="sxs-lookup"><span data-stu-id="16079-133">string</span></span>|<span data-ttu-id="16079-134">Schriftartname (z. B. "Calibri")</span><span class="sxs-lookup"><span data-stu-id="16079-134">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="16079-135">size</span><span class="sxs-lookup"><span data-stu-id="16079-135">size</span></span>|<span data-ttu-id="16079-136">double</span><span class="sxs-lookup"><span data-stu-id="16079-136">double</span></span>|<span data-ttu-id="16079-137">Der Schriftgrad (z. B. 11)</span><span class="sxs-lookup"><span data-stu-id="16079-137">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="16079-138">underline</span><span class="sxs-lookup"><span data-stu-id="16079-138">underline</span></span>|<span data-ttu-id="16079-139">string</span><span class="sxs-lookup"><span data-stu-id="16079-139">string</span></span>|<span data-ttu-id="16079-p103">Art der auf die Schriftart angewendeten Unterstreichung. Mögliche Werte: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="16079-p103">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16079-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="16079-142">Relationships</span></span>
<span data-ttu-id="16079-143">Keine</span><span class="sxs-lookup"><span data-stu-id="16079-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="16079-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="16079-144">JSON representation</span></span>

<span data-ttu-id="16079-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="16079-145">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
