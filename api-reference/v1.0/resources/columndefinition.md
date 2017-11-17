---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: e5942ddee4b505243cb64121862ce9e89e52d245
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="columndefinition-resource"></a><span data-ttu-id="97f2f-102">ColumnDefinition-Ressource</span><span class="sxs-lookup"><span data-stu-id="97f2f-102">ColumnDefinition resource</span></span>

## <a name="json-representation"></a><span data-ttu-id="97f2f-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="97f2f-103">JSON representation</span></span>

<span data-ttu-id="97f2f-104">Es folgt eine JSON-Darstellung einer ColumnDefinition-Ressource.</span><span class="sxs-lookup"><span data-stu-id="97f2f-104">Here is a JSON representation of a {type} resource.</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnDefinition",
       "keyProperty": "id", "optionalProperties": [ ] } -->

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
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a><span data-ttu-id="97f2f-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="97f2f-105">Properties</span></span>

<span data-ttu-id="97f2f-106">Die **ColumnDefinition**-Ressource weist folgende Eigenschaften auf.</span><span class="sxs-lookup"><span data-stu-id="97f2f-106">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="97f2f-107">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="97f2f-107">Property name</span></span>           | <span data-ttu-id="97f2f-108">Typ</span><span class="sxs-lookup"><span data-stu-id="97f2f-108">Type</span></span>    | <span data-ttu-id="97f2f-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97f2f-109">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="97f2f-110">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="97f2f-110">**columnGroup**</span></span>         | <span data-ttu-id="97f2f-111">string</span><span class="sxs-lookup"><span data-stu-id="97f2f-111">string</span></span>  | <span data-ttu-id="97f2f-112">Für Websitespalten der Name der Gruppe, zu der dieser Spalte gehört.</span><span class="sxs-lookup"><span data-stu-id="97f2f-112">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="97f2f-113">Dadurch können dazugehörige Spalten einfacher organisiert werden.</span><span class="sxs-lookup"><span data-stu-id="97f2f-113">Helps organize related columns.</span></span>
| <span data-ttu-id="97f2f-114">**description**</span><span class="sxs-lookup"><span data-stu-id="97f2f-114">**description**</span></span>         | <span data-ttu-id="97f2f-115">string</span><span class="sxs-lookup"><span data-stu-id="97f2f-115">string</span></span>  | <span data-ttu-id="97f2f-116">Für den Benutzer sichtbare Beschreibung der Spalte.</span><span class="sxs-lookup"><span data-stu-id="97f2f-116">The user-facing description of the column.</span></span>
| <span data-ttu-id="97f2f-117">**displayName**</span><span class="sxs-lookup"><span data-stu-id="97f2f-117">**displayName**</span></span>         | <span data-ttu-id="97f2f-118">string</span><span class="sxs-lookup"><span data-stu-id="97f2f-118">string</span></span>  | <span data-ttu-id="97f2f-119">Für den Benutzer sichtbarer Name der Spalte.</span><span class="sxs-lookup"><span data-stu-id="97f2f-119">The user-facing name of the column.</span></span>
| <span data-ttu-id="97f2f-120">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="97f2f-120">**enforceUniqueValues**</span></span> | <span data-ttu-id="97f2f-121">boolean</span><span class="sxs-lookup"><span data-stu-id="97f2f-121">boolean</span></span> | <span data-ttu-id="97f2f-122">Wenn der Wert true ist, dürfen keine der Elemente für diese Spalte den gleichen Wert aufweisen.</span><span class="sxs-lookup"><span data-stu-id="97f2f-122">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="97f2f-123">**hidden**</span><span class="sxs-lookup"><span data-stu-id="97f2f-123">**hidden**</span></span>              | <span data-ttu-id="97f2f-124">boolean</span><span class="sxs-lookup"><span data-stu-id="97f2f-124">boolean</span></span> | <span data-ttu-id="97f2f-125">Gibt an, ob die Spalte auf der Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="97f2f-125">Specifies the policy item name that is displayed in the oss14long user interface.</span></span>
| <span data-ttu-id="97f2f-126">**id**</span><span class="sxs-lookup"><span data-stu-id="97f2f-126">**id**</span></span>                  | <span data-ttu-id="97f2f-127">string</span><span class="sxs-lookup"><span data-stu-id="97f2f-127">string</span></span>  | <span data-ttu-id="97f2f-128">Die eindeutige ID für die Spalte.</span><span class="sxs-lookup"><span data-stu-id="97f2f-128">The unique identifier for the column.</span></span>
| <span data-ttu-id="97f2f-129">**indexed**</span><span class="sxs-lookup"><span data-stu-id="97f2f-129">**Indexed**</span></span>             | <span data-ttu-id="97f2f-130">boolean</span><span class="sxs-lookup"><span data-stu-id="97f2f-130">boolean</span></span> | <span data-ttu-id="97f2f-131">Gibt an, ob die Spaltenwerte für das Sortieren und Suchen verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="97f2f-131">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="97f2f-132">**name**</span><span class="sxs-lookup"><span data-stu-id="97f2f-132">**name**</span></span>                | <span data-ttu-id="97f2f-133">string</span><span class="sxs-lookup"><span data-stu-id="97f2f-133">string</span></span>  | <span data-ttu-id="97f2f-134">Der in der API sichtbare Name der Spalte, wie er in den  [Feldern][] eines [ListItem][] angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="97f2f-134">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="97f2f-135">Weitere Informationen zum für den Benutzer sichtbaren Namen finden Sie unter **displayName**.</span><span class="sxs-lookup"><span data-stu-id="97f2f-135">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="97f2f-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="97f2f-136">**Read-only.**</span></span>            | <span data-ttu-id="97f2f-137">bool</span><span class="sxs-lookup"><span data-stu-id="97f2f-137">bool</span></span>    | <span data-ttu-id="97f2f-138">Gibt an, ob die Werte in den Spalten geändert werden können.</span><span class="sxs-lookup"><span data-stu-id="97f2f-138">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="97f2f-139">**required**</span><span class="sxs-lookup"><span data-stu-id="97f2f-139">**Required**</span></span>            | <span data-ttu-id="97f2f-140">boolean</span><span class="sxs-lookup"><span data-stu-id="97f2f-140">boolean</span></span> | <span data-ttu-id="97f2f-141">Gibt an, ob die Werte in den Spalten obligatorisch sind.</span><span class="sxs-lookup"><span data-stu-id="97f2f-141">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="97f2f-142">Spalten können verschiedene Datentypen enthalten.</span><span class="sxs-lookup"><span data-stu-id="97f2f-142">Columns can hold data of various types.</span></span>
<span data-ttu-id="97f2f-143">Die folgenden Eigenschaften geben an, welche Arten von Daten in einer Spalte gespeichert werden sowie weitere Einstellungen für die Daten.</span><span class="sxs-lookup"><span data-stu-id="97f2f-143">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="97f2f-144">Diese Eigenschaften schließen sich gegenseitig aus – in einer Spalte kann nur eines der beiden angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="97f2f-144">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="97f2f-145">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="97f2f-145">Property name</span></span>     | <span data-ttu-id="97f2f-146">Typ</span><span class="sxs-lookup"><span data-stu-id="97f2f-146">Type</span></span>                    | <span data-ttu-id="97f2f-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97f2f-147">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="97f2f-148">**boolean**</span><span class="sxs-lookup"><span data-stu-id="97f2f-148">**Boolean**</span></span>       | <span data-ttu-id="97f2f-149">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="97f2f-149">[booleanColumn][]</span></span>       | <span data-ttu-id="97f2f-150">In dieser Spalte werden boolesche Werte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="97f2f-150">This column stores boolean values.</span></span>
| <span data-ttu-id="97f2f-151">**calculated**</span><span class="sxs-lookup"><span data-stu-id="97f2f-151">**Calculated**</span></span>    | <span data-ttu-id="97f2f-152">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="97f2f-152">[calculatedColumn][]</span></span>    | <span data-ttu-id="97f2f-153">Die Daten in dieser Spalte werden anhand von anderen Spalten berechnet.</span><span class="sxs-lookup"><span data-stu-id="97f2f-153">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="97f2f-154">**choice**</span><span class="sxs-lookup"><span data-stu-id="97f2f-154">**choice**</span></span>        | <span data-ttu-id="97f2f-155">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="97f2f-155">[choiceColumn][]</span></span>        | <span data-ttu-id="97f2f-156">In dieser Spalte werden Daten aus einer Auswahlliste gespeichert.</span><span class="sxs-lookup"><span data-stu-id="97f2f-156">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="97f2f-157">**currency**</span><span class="sxs-lookup"><span data-stu-id="97f2f-157">**Currency**</span></span>      | <span data-ttu-id="97f2f-158">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="97f2f-158">[currencyColumn][]</span></span>      | <span data-ttu-id="97f2f-159">In dieser Spalte sind die Währungswerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="97f2f-159">This column stores currency values.</span></span>
| <span data-ttu-id="97f2f-160">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="97f2f-160">**DateTime**</span></span>      | <span data-ttu-id="97f2f-161">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="97f2f-161">[dateTimeColumn][]</span></span>      | <span data-ttu-id="97f2f-162">In dieser Spalte sind die DateTime-Werte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="97f2f-162">This column stores DateTime values.</span></span>
| <span data-ttu-id="97f2f-163">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="97f2f-163">**defaultvalue**</span></span>  | <span data-ttu-id="97f2f-164">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="97f2f-164">[defaultColumnValue][]</span></span>  | <span data-ttu-id="97f2f-165">Der Standardwert für diese Spalte.</span><span class="sxs-lookup"><span data-stu-id="97f2f-165">The default value for this column.</span></span>
| <span data-ttu-id="97f2f-166">**lookup**</span><span class="sxs-lookup"><span data-stu-id="97f2f-166">**Lookup**</span></span>        | <span data-ttu-id="97f2f-167">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="97f2f-167">[lookupColumn][]</span></span>        | <span data-ttu-id="97f2f-168">Die Daten in dieser Spalte werden aus einer anderen Quelle dieser Website abgerufen.</span><span class="sxs-lookup"><span data-stu-id="97f2f-168">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="97f2f-169">**Zahl**</span><span class="sxs-lookup"><span data-stu-id="97f2f-169">**number**</span></span>        | <span data-ttu-id="97f2f-170">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="97f2f-170">[numberColumn][]</span></span>        | <span data-ttu-id="97f2f-171">In dieser Spalte werden Zahlenwerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="97f2f-171">This column stores number values.</span></span>
| <span data-ttu-id="97f2f-172">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="97f2f-172">**personOrGroup**</span></span> | <span data-ttu-id="97f2f-173">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="97f2f-173">[personOrGroupColumn][]</span></span> | <span data-ttu-id="97f2f-174">In dieser Spalte werden Personen- oder Gruppenwerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="97f2f-174">This column stores Person or Group values.</span></span>
| <span data-ttu-id="97f2f-175">**text**</span><span class="sxs-lookup"><span data-stu-id="97f2f-175">**text**</span></span>          | <span data-ttu-id="97f2f-176">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="97f2f-176">[textColumn][]</span></span>          | <span data-ttu-id="97f2f-177">In dieser Spalte werden Textwerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="97f2f-177">This column stores text values.</span></span>

<span data-ttu-id="97f2f-178">Hinweis: Diese Eigenschaften entsprechen der [SPFieldType][]-Enumeration von SharePoint.</span><span class="sxs-lookup"><span data-stu-id="97f2f-178">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="97f2f-179">Obwohl die meisten gängigen Feldtypen vorstehend dargestellt sind, fehlen bei dieser Beta-API noch einige.</span><span class="sxs-lookup"><span data-stu-id="97f2f-179">While the most common field types are represented above, this beta API is still missing some.</span></span>
<span data-ttu-id="97f2f-180">In diesen Fällen werden keine der Spaltentyp-Facets aufgefüllt und die Spalte weist nur die grundlegenden Eigenschaften auf.</span><span class="sxs-lookup"><span data-stu-id="97f2f-180">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="97f2f-181">Hinweise</span><span class="sxs-lookup"><span data-stu-id="97f2f-181">Remarks</span></span>

<span data-ttu-id="97f2f-182">ColumnDefinitions und Feldwerte für `hidden`-Spalten werden standardmäßig nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="97f2f-182">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="97f2f-183">Um diese bei der Auflistung von **ColumnDefinitions** anzuzeigen, fügen Sie `hidden` in Ihre `$select`-Anweisung ein.</span><span class="sxs-lookup"><span data-stu-id="97f2f-183">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="97f2f-184">Um diese beim Anzeigen von **field**-Werten mit [listItems][listItem] anzuzeigen, fügen Sie die gewünschten Spalten ein, indem Sie `$select` in Ihre Anweisung aufnehmen.</span><span class="sxs-lookup"><span data-stu-id="97f2f-184">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleanColumn.md
[calculatedColumn]: calculatedColumn.md
[choiceColumn]: choiceColumn.md
[currencyColumn]: currencyColumn.md
[dateTimeColumn]: dateTimeColumn.md
[defaultColumnValue]: defaultColumnValue.md
[lookupColumn]: lookupColumn.md
[numberColumn]: numberColumn.md
[personOrGroupColumn]: personOrGroupColumn.md
[textColumn]: textColumn.md
[fieldValueSet]: fieldValueSet.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

[SPFieldType]: https://msdn.microsoft.com/en-us/library/microsoft.sharepoint.spfieldtype.aspx

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
