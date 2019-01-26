---
title: Ressourcentyp WorkbookNamedItem
description: Stellt einen definierten Namen für einen Zellbereich oder einen Wert dar. Namen können einfach benannte Objekte (wie unten dargestellt), Bereichsobjekte, Verweise auf einen Bereich sein. Dieses Objekt kann zum Abrufen des mit Namen verknüpften Bereichsobjekts verwendet werden.
localization_priority: Normal
ms.openlocfilehash: 79ed5211c60555d2cfc55e01c49565ebecd58a8b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29579849"
---
# <a name="nameditem-resource-type"></a><span data-ttu-id="fc749-105">GetNamedItem Ressourcenart</span><span class="sxs-lookup"><span data-stu-id="fc749-105">NamedItem resource type</span></span>

<span data-ttu-id="fc749-p102">Stellt einen definierten Namen für einen Zellbereich oder einen Wert dar. Namen können einfach benannte Objekte (wie unten dargestellt), Bereichsobjekte, Verweise auf einen Bereich sein. Dieses Objekt kann zum Abrufen des mit Namen verknüpften Bereichsobjekts verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="fc749-p102">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="fc749-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="fc749-109">Methods</span></span>

| <span data-ttu-id="fc749-110">Methode</span><span class="sxs-lookup"><span data-stu-id="fc749-110">Method</span></span>           | <span data-ttu-id="fc749-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="fc749-111">Return Type</span></span>    |<span data-ttu-id="fc749-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc749-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fc749-113">Add</span><span class="sxs-lookup"><span data-stu-id="fc749-113">Add</span></span>](../api/nameditem-add.md)|[<span data-ttu-id="fc749-114">workbookNameditem</span><span class="sxs-lookup"><span data-stu-id="fc749-114">workbookNameditem</span></span>](workbooknameditem.md)|<span data-ttu-id="fc749-115">Fügt einen neuen Namen zur Auflistung des angegebenen Bereichs hinzu.</span><span class="sxs-lookup"><span data-stu-id="fc749-115">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="fc749-116">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="fc749-116">AddFormulaLocal</span></span>](../api/nameditem-addformulalocal.md)|[<span data-ttu-id="fc749-117">workbookNameditem</span><span class="sxs-lookup"><span data-stu-id="fc749-117">workbookNameditem</span></span>](workbooknameditem.md)|<span data-ttu-id="fc749-118">Fügt unter Verwendung des Gebietsschemas des Benutzers für die Formel einen neuen Namen zur Auflistung des angegebenen Bereichs hinzu.</span><span class="sxs-lookup"><span data-stu-id="fc749-118">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="fc749-119">NamedItem abrufen</span><span class="sxs-lookup"><span data-stu-id="fc749-119">Get NamedItem</span></span>](../api/nameditem-get.md) | [<span data-ttu-id="fc749-120">workbookNameditem</span><span class="sxs-lookup"><span data-stu-id="fc749-120">workbookNameditem</span></span>](workbooknameditem.md) |<span data-ttu-id="fc749-121">Dient zum Lesen der Eigenschaften und der Beziehungen des namedItem-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fc749-121">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="fc749-122">Update</span><span class="sxs-lookup"><span data-stu-id="fc749-122">Update</span></span>](../api/nameditem-update.md) | [<span data-ttu-id="fc749-123">workbookNameditem</span><span class="sxs-lookup"><span data-stu-id="fc749-123">workbookNameditem</span></span>](workbooknameditem.md)   |<span data-ttu-id="fc749-124">Dient zum Aktualisieren des NamedItem-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fc749-124">Update NamedItem object.</span></span> |
|[<span data-ttu-id="fc749-125">Range</span><span class="sxs-lookup"><span data-stu-id="fc749-125">Range</span></span>](../api/nameditem-range.md)|[<span data-ttu-id="fc749-126">range</span><span class="sxs-lookup"><span data-stu-id="fc749-126">range</span></span>](range.md)|<span data-ttu-id="fc749-p103">Ruft das Bereichsobjekt ab, das mit dem Namen verknüpft ist. Gibt eine Ausnahme zurück, wenn der Typ des benannten Elements kein Bereich ist.</span><span class="sxs-lookup"><span data-stu-id="fc749-p103">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="fc749-129">List</span><span class="sxs-lookup"><span data-stu-id="fc749-129">List</span></span>](../api/nameditem-list.md) | <span data-ttu-id="fc749-130">[WorkbookNameditem](workbooknameditem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="fc749-130">[workbookNameditem](workbooknameditem.md) collection</span></span> |<span data-ttu-id="fc749-131">Dient zum Abrufen einer der namedItem-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="fc749-131">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="fc749-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fc749-132">Properties</span></span>
| <span data-ttu-id="fc749-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fc749-133">Property</span></span>     | <span data-ttu-id="fc749-134">Typ</span><span class="sxs-lookup"><span data-stu-id="fc749-134">Type</span></span>   |<span data-ttu-id="fc749-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc749-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc749-136">name</span><span class="sxs-lookup"><span data-stu-id="fc749-136">name</span></span>|<span data-ttu-id="fc749-137">string</span><span class="sxs-lookup"><span data-stu-id="fc749-137">string</span></span>|<span data-ttu-id="fc749-p104">Der Name des Objekts. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fc749-p104">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="fc749-140">comment</span><span class="sxs-lookup"><span data-stu-id="fc749-140">comment</span></span>|<span data-ttu-id="fc749-141">string</span><span class="sxs-lookup"><span data-stu-id="fc749-141">string</span></span>|<span data-ttu-id="fc749-142">Stellt den Kommentar dar, der mit diesem Namen verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="fc749-142">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="fc749-143">scope</span><span class="sxs-lookup"><span data-stu-id="fc749-143">scope</span></span>|<span data-ttu-id="fc749-144">string</span><span class="sxs-lookup"><span data-stu-id="fc749-144">string</span></span>|<span data-ttu-id="fc749-p105">Gibt an, ob der Name im Bereich der Arbeitsmappe oder im Bereich eines bestimmten Arbeitsblatts liegt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fc749-p105">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="fc749-147">type</span><span class="sxs-lookup"><span data-stu-id="fc749-147">type</span></span>|<span data-ttu-id="fc749-148">string</span><span class="sxs-lookup"><span data-stu-id="fc749-148">string</span></span>|<span data-ttu-id="fc749-p106">Gibt an, welche Art von Verweis mit dem Namen verknüpft ist. Mögliche Werte:`String`, `Integer`, `Double`, `Boolean`, `Range`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fc749-p106">Indicates what type of reference is associated with the name. Possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`. Read-only.</span></span>|
|<span data-ttu-id="fc749-152">Wert</span><span class="sxs-lookup"><span data-stu-id="fc749-152">value</span></span>|<span data-ttu-id="fc749-153">string</span><span class="sxs-lookup"><span data-stu-id="fc749-153">string</span></span>|<span data-ttu-id="fc749-p107">Stellt die Formel dar, auf die der Name verweist. z. B. =Sheet14!$B$2:$H$12, =4.75 usw. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fc749-p107">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="fc749-157">visible</span><span class="sxs-lookup"><span data-stu-id="fc749-157">visible</span></span>|<span data-ttu-id="fc749-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="fc749-158">boolean</span></span>|<span data-ttu-id="fc749-159">Gibt an, ob das Objekt sichtbar ist.</span><span class="sxs-lookup"><span data-stu-id="fc749-159">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc749-160">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fc749-160">Relationships</span></span>
| <span data-ttu-id="fc749-161">Beziehung</span><span class="sxs-lookup"><span data-stu-id="fc749-161">Relationship</span></span>     | <span data-ttu-id="fc749-162">Typ</span><span class="sxs-lookup"><span data-stu-id="fc749-162">Type</span></span>   |<span data-ttu-id="fc749-163">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc749-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc749-164">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="fc749-164">worksheet</span></span>|[<span data-ttu-id="fc749-165">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="fc749-165">workbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="fc749-p108">Gibt das Arbeitsblatt zurück, auf dessen Bereich das benannte Element beschränkt ist. Nur verfügbar, wenn das Element auf das Arbeitsblatt beschränkt ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fc749-p108">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc749-169">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fc749-169">JSON representation</span></span>

<span data-ttu-id="fc749-170">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fc749-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookNamedItem"
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
