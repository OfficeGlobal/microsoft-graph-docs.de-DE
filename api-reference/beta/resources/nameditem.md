---
title: GetNamedItem Ressourcenart
description: Stellt einen definierten Namen für einen Zellbereich oder einen Wert dar. Namen können einfach benannte Objekte (wie unten dargestellt), Bereichsobjekte, Verweise auf einen Bereich sein. Dieses Objekt kann zum Abrufen des mit Namen verknüpften Bereichsobjekts verwendet werden.
localization_priority: Normal
ms.openlocfilehash: 5dd093976b2c09ae93c608144c8d6c2b7d7161c2
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649414"
---
# <a name="nameditem-resource-type"></a><span data-ttu-id="2dbe2-105">GetNamedItem Ressourcenart</span><span class="sxs-lookup"><span data-stu-id="2dbe2-105">NamedItem resource type</span></span>

<span data-ttu-id="2dbe2-p102">Stellt einen definierten Namen für einen Zellbereich oder einen Wert dar. Namen können einfach benannte Objekte (wie unten dargestellt), Bereichsobjekte, Verweise auf einen Bereich sein. Dieses Objekt kann zum Abrufen des mit Namen verknüpften Bereichsobjekts verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="2dbe2-p102">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="2dbe2-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="2dbe2-109">Methods</span></span>

| <span data-ttu-id="2dbe2-110">Methode</span><span class="sxs-lookup"><span data-stu-id="2dbe2-110">Method</span></span>           | <span data-ttu-id="2dbe2-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2dbe2-111">Return Type</span></span>    |<span data-ttu-id="2dbe2-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2dbe2-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2dbe2-113">Add</span><span class="sxs-lookup"><span data-stu-id="2dbe2-113">Add</span></span>](../api/nameditem-add.md)|[<span data-ttu-id="2dbe2-114">NamedItem</span><span class="sxs-lookup"><span data-stu-id="2dbe2-114">NamedItem</span></span>](nameditem.md)|<span data-ttu-id="2dbe2-115">Fügt einen neuen Namen zur Auflistung des angegebenen Bereichs hinzu.</span><span class="sxs-lookup"><span data-stu-id="2dbe2-115">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="2dbe2-116">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="2dbe2-116">AddFormulaLocal</span></span>](../api/nameditem-addformulalocal.md)|[<span data-ttu-id="2dbe2-117">NamedItem</span><span class="sxs-lookup"><span data-stu-id="2dbe2-117">NamedItem</span></span>](nameditem.md)|<span data-ttu-id="2dbe2-118">Fügt unter Verwendung des Gebietsschemas des Benutzers für die Formel einen neuen Namen zur Auflistung des angegebenen Bereichs hinzu.</span><span class="sxs-lookup"><span data-stu-id="2dbe2-118">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="2dbe2-119">NamedItem abrufen</span><span class="sxs-lookup"><span data-stu-id="2dbe2-119">Get NamedItem</span></span>](../api/nameditem-get.md) | [<span data-ttu-id="2dbe2-120">NamedItem</span><span class="sxs-lookup"><span data-stu-id="2dbe2-120">NamedItem</span></span>](nameditem.md) |<span data-ttu-id="2dbe2-121">Dient zum Lesen der Eigenschaften und der Beziehungen des namedItem-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2dbe2-121">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="2dbe2-122">Update</span><span class="sxs-lookup"><span data-stu-id="2dbe2-122">Update</span></span>](../api/nameditem-update.md) | [<span data-ttu-id="2dbe2-123">NamedItem</span><span class="sxs-lookup"><span data-stu-id="2dbe2-123">NamedItem</span></span>](nameditem.md)   |<span data-ttu-id="2dbe2-124">Dient zum Aktualisieren des NamedItem-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2dbe2-124">Update NamedItem object.</span></span> |
|[<span data-ttu-id="2dbe2-125">Range</span><span class="sxs-lookup"><span data-stu-id="2dbe2-125">Range</span></span>](../api/nameditem-range.md)|[<span data-ttu-id="2dbe2-126">Range</span><span class="sxs-lookup"><span data-stu-id="2dbe2-126">Range</span></span>](range.md)|<span data-ttu-id="2dbe2-p103">Ruft das Bereichsobjekt ab, das mit dem Namen verknüpft ist. Gibt eine Ausnahme zurück, wenn der Typ des benannten Elements kein Bereich ist.</span><span class="sxs-lookup"><span data-stu-id="2dbe2-p103">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="2dbe2-129">List</span><span class="sxs-lookup"><span data-stu-id="2dbe2-129">List</span></span>](../api/nameditem-list.md) | <span data-ttu-id="2dbe2-130">[NamedItem-Sammlung](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="2dbe2-130">[NamedItem](nameditem.md) collection</span></span> |<span data-ttu-id="2dbe2-131">Dient zum Abrufen einer der namedItem-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="2dbe2-131">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="2dbe2-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2dbe2-132">Properties</span></span>
| <span data-ttu-id="2dbe2-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2dbe2-133">Property</span></span>     | <span data-ttu-id="2dbe2-134">Typ</span><span class="sxs-lookup"><span data-stu-id="2dbe2-134">Type</span></span>   |<span data-ttu-id="2dbe2-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2dbe2-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2dbe2-136">name</span><span class="sxs-lookup"><span data-stu-id="2dbe2-136">name</span></span>|<span data-ttu-id="2dbe2-137">string</span><span class="sxs-lookup"><span data-stu-id="2dbe2-137">string</span></span>|<span data-ttu-id="2dbe2-p104">Der Name des Objekts. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2dbe2-p104">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="2dbe2-140">comment</span><span class="sxs-lookup"><span data-stu-id="2dbe2-140">comment</span></span>|<span data-ttu-id="2dbe2-141">string</span><span class="sxs-lookup"><span data-stu-id="2dbe2-141">string</span></span>|<span data-ttu-id="2dbe2-142">Stellt den Kommentar dar, der mit diesem Namen verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="2dbe2-142">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="2dbe2-143">scope</span><span class="sxs-lookup"><span data-stu-id="2dbe2-143">scope</span></span>|<span data-ttu-id="2dbe2-144">string</span><span class="sxs-lookup"><span data-stu-id="2dbe2-144">string</span></span>|<span data-ttu-id="2dbe2-p105">Gibt an, ob der Name im Bereich der Arbeitsmappe oder im Bereich eines bestimmten Arbeitsblatts liegt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2dbe2-p105">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="2dbe2-147">type</span><span class="sxs-lookup"><span data-stu-id="2dbe2-147">type</span></span>|<span data-ttu-id="2dbe2-148">string</span><span class="sxs-lookup"><span data-stu-id="2dbe2-148">string</span></span>|<span data-ttu-id="2dbe2-p106">Gibt an, welche Art von Verweis mit dem Namen verknüpft ist. Mögliche Werte:`String`, `Integer`, `Double`, `Boolean`, `Range`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2dbe2-p106">Indicates what type of reference is associated with the name. Possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`. Read-only.</span></span>|
|<span data-ttu-id="2dbe2-152">Wert</span><span class="sxs-lookup"><span data-stu-id="2dbe2-152">value</span></span>|<span data-ttu-id="2dbe2-153">string</span><span class="sxs-lookup"><span data-stu-id="2dbe2-153">string</span></span>|<span data-ttu-id="2dbe2-p107">Stellt die Formel dar, auf die der Name verweist. z. B. =Sheet14!$B$2:$H$12, =4.75 usw. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2dbe2-p107">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="2dbe2-157">visible</span><span class="sxs-lookup"><span data-stu-id="2dbe2-157">visible</span></span>|<span data-ttu-id="2dbe2-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2dbe2-158">boolean</span></span>|<span data-ttu-id="2dbe2-159">Gibt an, ob das Objekt sichtbar ist.</span><span class="sxs-lookup"><span data-stu-id="2dbe2-159">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2dbe2-160">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2dbe2-160">Relationships</span></span>
| <span data-ttu-id="2dbe2-161">Beziehung</span><span class="sxs-lookup"><span data-stu-id="2dbe2-161">Relationship</span></span>     | <span data-ttu-id="2dbe2-162">Typ</span><span class="sxs-lookup"><span data-stu-id="2dbe2-162">Type</span></span>   |<span data-ttu-id="2dbe2-163">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2dbe2-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2dbe2-164">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="2dbe2-164">worksheet</span></span>|[<span data-ttu-id="2dbe2-165">worksheet</span><span class="sxs-lookup"><span data-stu-id="2dbe2-165">worksheet</span></span>](worksheet.md)|<span data-ttu-id="2dbe2-p108">Gibt das Arbeitsblatt zurück, auf dessen Bereich das benannte Element beschränkt ist. Nur verfügbar, wenn das Element auf das Arbeitsblatt beschränkt ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2dbe2-p108">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2dbe2-169">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2dbe2-169">JSON representation</span></span>

<span data-ttu-id="2dbe2-170">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2dbe2-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": "string",
  "visible": true
  
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
