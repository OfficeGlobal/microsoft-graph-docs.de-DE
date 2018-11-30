---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: 9b99abe78b009786d489ec7f0c0fdce1e2945b1d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058277"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="e175d-102">ColumnDefinition Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e175d-102">columnDefinition resource type</span></span>

> <span data-ttu-id="e175d-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e175d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e175d-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e175d-104">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e175d-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e175d-105">JSON representation</span></span>

<span data-ttu-id="e175d-106">Es folgt eine JSON-Darstellung einer Ressource ColumnDefinition.</span><span class="sxs-lookup"><span data-stu-id="e175d-106">Here is a JSON representation of a columnDefinition resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnDefinition"
}-->

```json
{
  "columnGroup": "string",
  "description": "description",
  "displayName": "friendly name",
  "enforceUniqueValues": "true",
  "hidden": false,
  "id": "string",
  "indexed": true,
  "name": "staticNameForApi",
  "readOnly": false,
  "required": false,
  "boolean": { "@odata.type": "microsoft.graph.booleanColumn" },
  "calculated": { "@odata.type": "microsoft.graph.calculatedColumn" },
  "choice": { "@odata.type": "microsoft.graph.choiceColumn" },
  "currency": { "@odata.type": "microsoft.graph.currencyColumn" },
  "dateTime": { "@odata.type": "microsoft.graph.dateTimeColumn" },
  "defaultValue": { "@odata.type": "microsoft.graph.defaultColumnValue" },
  "geolocation": { "@odata.type": "microsoft.graph.geolocationColumn" },
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a><span data-ttu-id="e175d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e175d-107">Properties</span></span>

<span data-ttu-id="e175d-108">Spalten können verschiedene Datentypen enthalten.</span><span class="sxs-lookup"><span data-stu-id="e175d-108">Columns can hold data of various types.</span></span>
<span data-ttu-id="e175d-109">Die folgenden Eigenschaften geben an, welche Arten von Daten in einer Spalte gespeichert werden sowie weitere Einstellungen für die Daten.</span><span class="sxs-lookup"><span data-stu-id="e175d-109">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="e175d-110">Die Typ-bezogene Eigenschaften (boolean, berechnet, Auswahl, Währung, DateTime, Suche, Anzahl, PersonOrGroup, Text) schließen sich gegenseitig aus – eine Spalte kann nur einer von ihnen angegeben haben.</span><span class="sxs-lookup"><span data-stu-id="e175d-110">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="e175d-111">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="e175d-111">Property name</span></span>           | <span data-ttu-id="e175d-112">Typ</span><span class="sxs-lookup"><span data-stu-id="e175d-112">Type</span></span>    | <span data-ttu-id="e175d-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e175d-113">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="e175d-114">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="e175d-114">**columnGroup**</span></span>         | <span data-ttu-id="e175d-115">string</span><span class="sxs-lookup"><span data-stu-id="e175d-115">string</span></span>  | <span data-ttu-id="e175d-116">Für Websitespalten der Name der Gruppe, zu der dieser Spalte gehört.</span><span class="sxs-lookup"><span data-stu-id="e175d-116">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="e175d-117">Dadurch können dazugehörige Spalten einfacher organisiert werden.</span><span class="sxs-lookup"><span data-stu-id="e175d-117">Helps organize related columns.</span></span>
| <span data-ttu-id="e175d-118">**description**</span><span class="sxs-lookup"><span data-stu-id="e175d-118">**description**</span></span>         | <span data-ttu-id="e175d-119">string</span><span class="sxs-lookup"><span data-stu-id="e175d-119">string</span></span>  | <span data-ttu-id="e175d-120">Für den Benutzer sichtbare Beschreibung der Spalte.</span><span class="sxs-lookup"><span data-stu-id="e175d-120">The user-facing description of the column.</span></span>
| <span data-ttu-id="e175d-121">**displayName**</span><span class="sxs-lookup"><span data-stu-id="e175d-121">**displayName**</span></span>         | <span data-ttu-id="e175d-122">string</span><span class="sxs-lookup"><span data-stu-id="e175d-122">string</span></span>  | <span data-ttu-id="e175d-123">Für den Benutzer sichtbarer Name der Spalte.</span><span class="sxs-lookup"><span data-stu-id="e175d-123">The user-facing name of the column.</span></span>
| <span data-ttu-id="e175d-124">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="e175d-124">**enforceUniqueValues**</span></span> | <span data-ttu-id="e175d-125">boolean</span><span class="sxs-lookup"><span data-stu-id="e175d-125">boolean</span></span> | <span data-ttu-id="e175d-126">Wenn der Wert true ist, dürfen keine der Elemente für diese Spalte den gleichen Wert aufweisen.</span><span class="sxs-lookup"><span data-stu-id="e175d-126">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="e175d-127">**hidden**</span><span class="sxs-lookup"><span data-stu-id="e175d-127">**hidden**</span></span>              | <span data-ttu-id="e175d-128">boolean</span><span class="sxs-lookup"><span data-stu-id="e175d-128">boolean</span></span> | <span data-ttu-id="e175d-129">Gibt an, ob die Spalte auf der Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e175d-129">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="e175d-130">**id**</span><span class="sxs-lookup"><span data-stu-id="e175d-130">**id**</span></span>                  | <span data-ttu-id="e175d-131">string</span><span class="sxs-lookup"><span data-stu-id="e175d-131">string</span></span>  | <span data-ttu-id="e175d-132">Die eindeutige ID für die Spalte.</span><span class="sxs-lookup"><span data-stu-id="e175d-132">The unique identifier for the column.</span></span>
| <span data-ttu-id="e175d-133">**indexed**</span><span class="sxs-lookup"><span data-stu-id="e175d-133">**indexed**</span></span>             | <span data-ttu-id="e175d-134">boolean</span><span class="sxs-lookup"><span data-stu-id="e175d-134">boolean</span></span> | <span data-ttu-id="e175d-135">Gibt an, ob die Spaltenwerte für das Sortieren und Suchen verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="e175d-135">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="e175d-136">**name**</span><span class="sxs-lookup"><span data-stu-id="e175d-136">**name**</span></span>                | <span data-ttu-id="e175d-137">string</span><span class="sxs-lookup"><span data-stu-id="e175d-137">string</span></span>  | <span data-ttu-id="e175d-138">Der in der API sichtbare Name der Spalte, wie er in den  [Feldern][] eines [ListItem][] angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e175d-138">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="e175d-139">Weitere Informationen zum für den Benutzer sichtbaren Namen finden Sie unter **displayName**.</span><span class="sxs-lookup"><span data-stu-id="e175d-139">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="e175d-140">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="e175d-140">**readOnly**</span></span>            | <span data-ttu-id="e175d-141">bool</span><span class="sxs-lookup"><span data-stu-id="e175d-141">bool</span></span>    | <span data-ttu-id="e175d-142">Gibt an, ob die Werte in den Spalten geändert werden können.</span><span class="sxs-lookup"><span data-stu-id="e175d-142">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="e175d-143">**required**</span><span class="sxs-lookup"><span data-stu-id="e175d-143">**required**</span></span>            | <span data-ttu-id="e175d-144">boolean</span><span class="sxs-lookup"><span data-stu-id="e175d-144">boolean</span></span> | <span data-ttu-id="e175d-145">Gibt an, ob die Werte in den Spalten obligatorisch sind.</span><span class="sxs-lookup"><span data-stu-id="e175d-145">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="e175d-146">**boolean**</span><span class="sxs-lookup"><span data-stu-id="e175d-146">**boolean**</span></span>       | <span data-ttu-id="e175d-147">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="e175d-147">[booleanColumn][]</span></span>       | <span data-ttu-id="e175d-148">In dieser Spalte werden boolesche Werte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="e175d-148">This column stores boolean values.</span></span>
| <span data-ttu-id="e175d-149">**calculated**</span><span class="sxs-lookup"><span data-stu-id="e175d-149">**calculated**</span></span>    | <span data-ttu-id="e175d-150">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="e175d-150">[calculatedColumn][]</span></span>    | <span data-ttu-id="e175d-151">Die Daten in dieser Spalte werden anhand von anderen Spalten berechnet.</span><span class="sxs-lookup"><span data-stu-id="e175d-151">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="e175d-152">**choice**</span><span class="sxs-lookup"><span data-stu-id="e175d-152">**choice**</span></span>        | <span data-ttu-id="e175d-153">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="e175d-153">[choiceColumn][]</span></span>        | <span data-ttu-id="e175d-154">In dieser Spalte werden Daten aus einer Auswahlliste gespeichert.</span><span class="sxs-lookup"><span data-stu-id="e175d-154">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="e175d-155">**currency**</span><span class="sxs-lookup"><span data-stu-id="e175d-155">**currency**</span></span>      | <span data-ttu-id="e175d-156">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="e175d-156">[currencyColumn][]</span></span>      | <span data-ttu-id="e175d-157">In dieser Spalte sind die Währungswerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="e175d-157">This column stores currency values.</span></span>
| <span data-ttu-id="e175d-158">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="e175d-158">**dateTime**</span></span>      | <span data-ttu-id="e175d-159">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="e175d-159">[dateTimeColumn][]</span></span>      | <span data-ttu-id="e175d-160">In dieser Spalte sind die DateTime-Werte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="e175d-160">This column stores DateTime values.</span></span>
| <span data-ttu-id="e175d-161">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="e175d-161">**defaultValue**</span></span>  | <span data-ttu-id="e175d-162">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="e175d-162">[defaultColumnValue][]</span></span>  | <span data-ttu-id="e175d-163">Der Standardwert für diese Spalte.</span><span class="sxs-lookup"><span data-stu-id="e175d-163">The default value for this column.</span></span>
| <span data-ttu-id="e175d-164">**GeoLocation**</span><span class="sxs-lookup"><span data-stu-id="e175d-164">**geolocation**</span></span>   | <span data-ttu-id="e175d-165">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="e175d-165">[geolocationColumn][]</span></span>   | <span data-ttu-id="e175d-166">Diese Spalte speichert ein GeoLocation-Objekt.</span><span class="sxs-lookup"><span data-stu-id="e175d-166">This column stores a geolocation.</span></span>
| <span data-ttu-id="e175d-167">**lookup**</span><span class="sxs-lookup"><span data-stu-id="e175d-167">**lookup**</span></span>        | <span data-ttu-id="e175d-168">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="e175d-168">[lookupColumn][]</span></span>        | <span data-ttu-id="e175d-169">Die Daten in dieser Spalte werden aus einer anderen Quelle dieser Website abgerufen.</span><span class="sxs-lookup"><span data-stu-id="e175d-169">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="e175d-170">**number**</span><span class="sxs-lookup"><span data-stu-id="e175d-170">**number**</span></span>        | <span data-ttu-id="e175d-171">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="e175d-171">[numberColumn][]</span></span>        | <span data-ttu-id="e175d-172">In dieser Spalte werden Zahlenwerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="e175d-172">This column stores number values.</span></span>
| <span data-ttu-id="e175d-173">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="e175d-173">**personOrGroup**</span></span> | <span data-ttu-id="e175d-174">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="e175d-174">[personOrGroupColumn][]</span></span> | <span data-ttu-id="e175d-175">In dieser Spalte werden Personen- oder Gruppenwerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="e175d-175">This column stores Person or Group values.</span></span>
| <span data-ttu-id="e175d-176">**text**</span><span class="sxs-lookup"><span data-stu-id="e175d-176">**text**</span></span>          | <span data-ttu-id="e175d-177">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="e175d-177">[textColumn][]</span></span>          | <span data-ttu-id="e175d-178">In dieser Spalte werden Textwerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="e175d-178">This column stores text values.</span></span>

><span data-ttu-id="e175d-179">**Hinweis:** Diese Eigenschaften entsprechen SharePoint [SPFieldType][] -Enumeration.</span><span class="sxs-lookup"><span data-stu-id="e175d-179">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="e175d-180">Während die am häufigsten verwendeten Feldtypen in der vorherigen Tabelle dargestellt werden, ist dieses Beta API noch einige fehlt.</span><span class="sxs-lookup"><span data-stu-id="e175d-180">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="e175d-181">In diesen Fällen werden keine der Spaltentyp-Facets aufgefüllt und die Spalte weist nur die grundlegenden Eigenschaften auf.</span><span class="sxs-lookup"><span data-stu-id="e175d-181">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="e175d-182">Hinweise</span><span class="sxs-lookup"><span data-stu-id="e175d-182">Remarks</span></span>

<span data-ttu-id="e175d-183">ColumnDefinitions und Feldwerte für `hidden`-Spalten werden standardmäßig nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e175d-183">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="e175d-184">Um diese bei der Auflistung von **ColumnDefinitions** anzuzeigen, fügen Sie `hidden` in Ihre `$select`-Anweisung ein.</span><span class="sxs-lookup"><span data-stu-id="e175d-184">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="e175d-185">Um diese beim Anzeigen von **field**-Werten mit [listItems][listItem] anzuzeigen, fügen Sie die gewünschten Spalten ein, indem Sie `$select` in Ihre Anweisung aufnehmen.</span><span class="sxs-lookup"><span data-stu-id="e175d-185">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[geolocationColumn]: geolocationcolumn.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

<span data-ttu-id="e175d-199">
  [SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span><span class="sxs-lookup"><span data-stu-id="e175d-199">[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
