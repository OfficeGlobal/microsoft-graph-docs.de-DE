---
title: GetNamedItem Ressourcenart
description: Stellt einen definierten Namen für einen Zellbereich oder einen Wert dar. Namen können einfach benannte Objekte (wie unten dargestellt), Bereichsobjekte, Verweise auf einen Bereich sein. Dieses Objekt kann zum Abrufen des mit Namen verknüpften Bereichsobjekts verwendet werden.
ms.openlocfilehash: 683bc93fdd9c14005b70cb125cf09eba5c8075a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020000"
---
# <a name="nameditem-resource-type"></a><span data-ttu-id="80bc1-105">GetNamedItem Ressourcenart</span><span class="sxs-lookup"><span data-stu-id="80bc1-105">NamedItem resource type</span></span>

<span data-ttu-id="80bc1-p102">Stellt einen definierten Namen für einen Zellbereich oder einen Wert dar. Namen können einfach benannte Objekte (wie unten dargestellt), Bereichsobjekte, Verweise auf einen Bereich sein. Dieses Objekt kann zum Abrufen des mit Namen verknüpften Bereichsobjekts verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="80bc1-p102">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="80bc1-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="80bc1-109">Methods</span></span>

| <span data-ttu-id="80bc1-110">Methode</span><span class="sxs-lookup"><span data-stu-id="80bc1-110">Method</span></span>           | <span data-ttu-id="80bc1-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="80bc1-111">Return Type</span></span>    |<span data-ttu-id="80bc1-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80bc1-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="80bc1-113">Add</span><span class="sxs-lookup"><span data-stu-id="80bc1-113">Add</span></span>](../api/nameditem-add.md)|[<span data-ttu-id="80bc1-114">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="80bc1-114">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="80bc1-115">Fügt einen neuen Namen zur Auflistung des angegebenen Bereichs hinzu.</span><span class="sxs-lookup"><span data-stu-id="80bc1-115">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="80bc1-116">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="80bc1-116">AddFormulaLocal</span></span>](../api/nameditem-addformulalocal.md)|[<span data-ttu-id="80bc1-117">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="80bc1-117">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="80bc1-118">Fügt unter Verwendung des Gebietsschemas des Benutzers für die Formel einen neuen Namen zur Auflistung des angegebenen Bereichs hinzu.</span><span class="sxs-lookup"><span data-stu-id="80bc1-118">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="80bc1-119">NamedItem abrufen</span><span class="sxs-lookup"><span data-stu-id="80bc1-119">Get NamedItem</span></span>](../api/nameditem-get.md) | [<span data-ttu-id="80bc1-120">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="80bc1-120">WorkbookNamedItem</span></span>](nameditem.md) |<span data-ttu-id="80bc1-121">Dient zum Lesen der Eigenschaften und der Beziehungen des namedItem-Objekts.</span><span class="sxs-lookup"><span data-stu-id="80bc1-121">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="80bc1-122">Update</span><span class="sxs-lookup"><span data-stu-id="80bc1-122">Update</span></span>](../api/nameditem-update.md) | [<span data-ttu-id="80bc1-123">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="80bc1-123">WorkbookNamedItem</span></span>](nameditem.md)   |<span data-ttu-id="80bc1-124">Dient zum Aktualisieren des NamedItem-Objekts.</span><span class="sxs-lookup"><span data-stu-id="80bc1-124">Update NamedItem object.</span></span> |
|[<span data-ttu-id="80bc1-125">Range</span><span class="sxs-lookup"><span data-stu-id="80bc1-125">Range</span></span>](../api/nameditem-range.md)|[<span data-ttu-id="80bc1-126">Range</span><span class="sxs-lookup"><span data-stu-id="80bc1-126">Range</span></span>](range.md)|<span data-ttu-id="80bc1-p103">Ruft das Bereichsobjekt ab, das mit dem Namen verknüpft ist. Gibt eine Ausnahme zurück, wenn der Typ des benannten Elements kein Bereich ist.</span><span class="sxs-lookup"><span data-stu-id="80bc1-p103">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="80bc1-129">List</span><span class="sxs-lookup"><span data-stu-id="80bc1-129">List</span></span>](../api/nameditem-list.md) | <span data-ttu-id="80bc1-130">[WorkbookNamedItem](nameditem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="80bc1-130">[WorkbookNamedItem](nameditem.md) collection</span></span> |<span data-ttu-id="80bc1-131">Dient zum Abrufen einer der namedItem-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="80bc1-131">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="80bc1-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="80bc1-132">Properties</span></span>
| <span data-ttu-id="80bc1-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="80bc1-133">Property</span></span>     | <span data-ttu-id="80bc1-134">Typ</span><span class="sxs-lookup"><span data-stu-id="80bc1-134">Type</span></span>   |<span data-ttu-id="80bc1-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80bc1-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80bc1-136">name</span><span class="sxs-lookup"><span data-stu-id="80bc1-136">name</span></span>|<span data-ttu-id="80bc1-137">string</span><span class="sxs-lookup"><span data-stu-id="80bc1-137">string</span></span>|<span data-ttu-id="80bc1-p104">Der Name des Objekts. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="80bc1-p104">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="80bc1-140">comment</span><span class="sxs-lookup"><span data-stu-id="80bc1-140">comment</span></span>|<span data-ttu-id="80bc1-141">string</span><span class="sxs-lookup"><span data-stu-id="80bc1-141">string</span></span>|<span data-ttu-id="80bc1-142">Stellt den Kommentar dar, der mit diesem Namen verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="80bc1-142">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="80bc1-143">scope</span><span class="sxs-lookup"><span data-stu-id="80bc1-143">scope</span></span>|<span data-ttu-id="80bc1-144">string</span><span class="sxs-lookup"><span data-stu-id="80bc1-144">string</span></span>|<span data-ttu-id="80bc1-p105">Gibt an, ob der Name im Bereich der Arbeitsmappe oder im Bereich eines bestimmten Arbeitsblatts liegt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="80bc1-p105">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="80bc1-147">type</span><span class="sxs-lookup"><span data-stu-id="80bc1-147">type</span></span>|<span data-ttu-id="80bc1-148">string</span><span class="sxs-lookup"><span data-stu-id="80bc1-148">string</span></span>|<span data-ttu-id="80bc1-149">Gibt an, welche Art von Bezug den Namen zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="80bc1-149">Indicates what type of reference is associated with the name.</span></span> <span data-ttu-id="80bc1-150">Die möglichen Werte sind: `String`, `Integer`, `Double`, `Boolean`, `Range`.</span><span class="sxs-lookup"><span data-stu-id="80bc1-150">The possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`.</span></span> <span data-ttu-id="80bc1-151">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="80bc1-151">Read-only.</span></span>|
|<span data-ttu-id="80bc1-152">Wert</span><span class="sxs-lookup"><span data-stu-id="80bc1-152">value</span></span>|<span data-ttu-id="80bc1-153">Json</span><span class="sxs-lookup"><span data-stu-id="80bc1-153">Json</span></span>|<span data-ttu-id="80bc1-p107">Stellt die Formel dar, auf die der Name verweist. z. B. =Sheet14!$B$2:$H$12, =4.75 usw. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="80bc1-p107">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="80bc1-157">visible</span><span class="sxs-lookup"><span data-stu-id="80bc1-157">visible</span></span>|<span data-ttu-id="80bc1-158">boolean</span><span class="sxs-lookup"><span data-stu-id="80bc1-158">boolean</span></span>|<span data-ttu-id="80bc1-159">Gibt an, ob das Objekt sichtbar ist.</span><span class="sxs-lookup"><span data-stu-id="80bc1-159">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80bc1-160">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="80bc1-160">Relationships</span></span>
| <span data-ttu-id="80bc1-161">Beziehung</span><span class="sxs-lookup"><span data-stu-id="80bc1-161">Relationship</span></span>     | <span data-ttu-id="80bc1-162">Typ</span><span class="sxs-lookup"><span data-stu-id="80bc1-162">Type</span></span>   |<span data-ttu-id="80bc1-163">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80bc1-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80bc1-164">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="80bc1-164">worksheet</span></span>|[<span data-ttu-id="80bc1-165">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="80bc1-165">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="80bc1-p108">Gibt das Arbeitsblatt zurück, auf dessen Bereich das benannte Element beschränkt ist. Nur verfügbar, wenn das Element auf das Arbeitsblatt beschränkt ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="80bc1-p108">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="80bc1-169">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="80bc1-169">JSON representation</span></span>

<span data-ttu-id="80bc1-170">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="80bc1-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookNamedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": {"@odata.type": "microsoft.graph.Json"},
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
