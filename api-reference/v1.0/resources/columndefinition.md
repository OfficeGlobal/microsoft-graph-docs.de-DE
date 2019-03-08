---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
ms.openlocfilehash: 679f0139f7ad0e94eab1970cc113268a56722663
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481881"
---
# <a name="columndefinition-resource"></a><span data-ttu-id="d1484-102">ColumnDefinition-Ressource</span><span class="sxs-lookup"><span data-stu-id="d1484-102">ColumnDefinition resource</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1484-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d1484-103">JSON representation</span></span>

<span data-ttu-id="d1484-104">Es folgt eine JSON-Darstellung einer ColumnDefinition-Ressource.</span><span class="sxs-lookup"><span data-stu-id="d1484-104">Here is a JSON representation of a ColumnDefinition resource.</span></span>

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
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a><span data-ttu-id="d1484-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d1484-105">Properties</span></span>

<span data-ttu-id="d1484-106">Die **ColumnDefinition**-Ressource weist folgende Eigenschaften auf.</span><span class="sxs-lookup"><span data-stu-id="d1484-106">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="d1484-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="d1484-107">Property name</span></span>           | <span data-ttu-id="d1484-108">Typ</span><span class="sxs-lookup"><span data-stu-id="d1484-108">Type</span></span>    | <span data-ttu-id="d1484-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1484-109">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="d1484-110">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="d1484-110">**columnGroup**</span></span>         | <span data-ttu-id="d1484-111">string</span><span class="sxs-lookup"><span data-stu-id="d1484-111">string</span></span>  | <span data-ttu-id="d1484-112">Für Websitespalten der Name der Gruppe, zu der dieser Spalte gehört.</span><span class="sxs-lookup"><span data-stu-id="d1484-112">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="d1484-113">Dadurch können dazugehörige Spalten einfacher organisiert werden.</span><span class="sxs-lookup"><span data-stu-id="d1484-113">Helps organize related columns.</span></span>
| <span data-ttu-id="d1484-114">**description**</span><span class="sxs-lookup"><span data-stu-id="d1484-114">**description**</span></span>         | <span data-ttu-id="d1484-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1484-115">string</span></span>  | <span data-ttu-id="d1484-116">Für den Benutzer sichtbare Beschreibung der Spalte.</span><span class="sxs-lookup"><span data-stu-id="d1484-116">The user-facing description of the column.</span></span>
| <span data-ttu-id="d1484-117">**displayName**</span><span class="sxs-lookup"><span data-stu-id="d1484-117">**displayName**</span></span>         | <span data-ttu-id="d1484-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1484-118">string</span></span>  | <span data-ttu-id="d1484-119">Für den Benutzer sichtbarer Name der Spalte.</span><span class="sxs-lookup"><span data-stu-id="d1484-119">The user-facing name of the column.</span></span>
| <span data-ttu-id="d1484-120">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="d1484-120">**enforceUniqueValues**</span></span> | <span data-ttu-id="d1484-121">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d1484-121">boolean</span></span> | <span data-ttu-id="d1484-122">Wenn der Wert true ist, dürfen keine der Elemente für diese Spalte den gleichen Wert aufweisen.</span><span class="sxs-lookup"><span data-stu-id="d1484-122">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="d1484-123">**hidden**</span><span class="sxs-lookup"><span data-stu-id="d1484-123">**hidden**</span></span>              | <span data-ttu-id="d1484-124">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d1484-124">boolean</span></span> | <span data-ttu-id="d1484-125">Gibt an, ob die Spalte auf der Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="d1484-125">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="d1484-126">**id**</span><span class="sxs-lookup"><span data-stu-id="d1484-126">**id**</span></span>                  | <span data-ttu-id="d1484-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1484-127">string</span></span>  | <span data-ttu-id="d1484-128">Die eindeutige ID für die Spalte.</span><span class="sxs-lookup"><span data-stu-id="d1484-128">The unique identifier for the column.</span></span>
| <span data-ttu-id="d1484-129">**indexed**</span><span class="sxs-lookup"><span data-stu-id="d1484-129">**indexed**</span></span>             | <span data-ttu-id="d1484-130">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d1484-130">boolean</span></span> | <span data-ttu-id="d1484-131">Gibt an, ob die Spaltenwerte für das Sortieren und Suchen verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="d1484-131">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="d1484-132">**name**</span><span class="sxs-lookup"><span data-stu-id="d1484-132">**name**</span></span>                | <span data-ttu-id="d1484-133">string</span><span class="sxs-lookup"><span data-stu-id="d1484-133">string</span></span>  | <span data-ttu-id="d1484-134">Der in der API sichtbare Name der Spalte, wie er in den  [Feldern][] eines [ListItem][] angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="d1484-134">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="d1484-135">Weitere Informationen zum für den Benutzer sichtbaren Namen finden Sie unter **displayName**.</span><span class="sxs-lookup"><span data-stu-id="d1484-135">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="d1484-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="d1484-136">**readOnly**</span></span>            | <span data-ttu-id="d1484-137">bool</span><span class="sxs-lookup"><span data-stu-id="d1484-137">bool</span></span>    | <span data-ttu-id="d1484-138">Gibt an, ob die Werte in den Spalten geändert werden können.</span><span class="sxs-lookup"><span data-stu-id="d1484-138">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="d1484-139">**required**</span><span class="sxs-lookup"><span data-stu-id="d1484-139">**required**</span></span>            | <span data-ttu-id="d1484-140">boolean</span><span class="sxs-lookup"><span data-stu-id="d1484-140">boolean</span></span> | <span data-ttu-id="d1484-141">Gibt an, ob die Werte in den Spalten obligatorisch sind.</span><span class="sxs-lookup"><span data-stu-id="d1484-141">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="d1484-142">Spalten können verschiedene Datentypen enthalten.</span><span class="sxs-lookup"><span data-stu-id="d1484-142">Columns can hold data of various types.</span></span>
<span data-ttu-id="d1484-143">Die folgenden Eigenschaften geben an, welche Arten von Daten in einer Spalte gespeichert werden sowie weitere Einstellungen für die Daten.</span><span class="sxs-lookup"><span data-stu-id="d1484-143">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="d1484-144">Diese Eigenschaften schließen sich gegenseitig aus – in einer Spalte kann nur eines der beiden angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="d1484-144">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="d1484-145">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="d1484-145">Property name</span></span>     | <span data-ttu-id="d1484-146">Typ</span><span class="sxs-lookup"><span data-stu-id="d1484-146">Type</span></span>                    | <span data-ttu-id="d1484-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1484-147">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="d1484-148">**boolean**</span><span class="sxs-lookup"><span data-stu-id="d1484-148">**boolean**</span></span>       | <span data-ttu-id="d1484-149">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="d1484-149">[booleanColumn][]</span></span>       | <span data-ttu-id="d1484-150">In dieser Spalte werden boolesche Werte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="d1484-150">This column stores boolean values.</span></span>
| <span data-ttu-id="d1484-151">**calculated**</span><span class="sxs-lookup"><span data-stu-id="d1484-151">**calculated**</span></span>    | <span data-ttu-id="d1484-152">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="d1484-152">[calculatedColumn][]</span></span>    | <span data-ttu-id="d1484-153">Die Daten in dieser Spalte werden anhand von anderen Spalten berechnet.</span><span class="sxs-lookup"><span data-stu-id="d1484-153">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="d1484-154">**choice**</span><span class="sxs-lookup"><span data-stu-id="d1484-154">**choice**</span></span>        | <span data-ttu-id="d1484-155">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="d1484-155">[choiceColumn][]</span></span>        | <span data-ttu-id="d1484-156">In dieser Spalte werden Daten aus einer Auswahlliste gespeichert.</span><span class="sxs-lookup"><span data-stu-id="d1484-156">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="d1484-157">**currency**</span><span class="sxs-lookup"><span data-stu-id="d1484-157">**currency**</span></span>      | <span data-ttu-id="d1484-158">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="d1484-158">[currencyColumn][]</span></span>      | <span data-ttu-id="d1484-159">In dieser Spalte sind die Währungswerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="d1484-159">This column stores currency values.</span></span>
| <span data-ttu-id="d1484-160">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="d1484-160">**dateTime**</span></span>      | <span data-ttu-id="d1484-161">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="d1484-161">[dateTimeColumn][]</span></span>      | <span data-ttu-id="d1484-162">In dieser Spalte sind die DateTime-Werte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="d1484-162">This column stores DateTime values.</span></span>
| <span data-ttu-id="d1484-163">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="d1484-163">**defaultValue**</span></span>  | <span data-ttu-id="d1484-164">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="d1484-164">[defaultColumnValue][]</span></span>  | <span data-ttu-id="d1484-165">Der Standardwert für diese Spalte.</span><span class="sxs-lookup"><span data-stu-id="d1484-165">The default value for this column.</span></span>
| <span data-ttu-id="d1484-166">**lookup**</span><span class="sxs-lookup"><span data-stu-id="d1484-166">**lookup**</span></span>        | <span data-ttu-id="d1484-167">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="d1484-167">[lookupColumn][]</span></span>        | <span data-ttu-id="d1484-168">Die Daten in dieser Spalte werden aus einer anderen Quelle dieser Website abgerufen.</span><span class="sxs-lookup"><span data-stu-id="d1484-168">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="d1484-169">**number**</span><span class="sxs-lookup"><span data-stu-id="d1484-169">**number**</span></span>        | <span data-ttu-id="d1484-170">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="d1484-170">[numberColumn][]</span></span>        | <span data-ttu-id="d1484-171">In dieser Spalte werden Zahlenwerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="d1484-171">This column stores number values.</span></span>
| <span data-ttu-id="d1484-172">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="d1484-172">**personOrGroup**</span></span> | <span data-ttu-id="d1484-173">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="d1484-173">[personOrGroupColumn][]</span></span> | <span data-ttu-id="d1484-174">In dieser Spalte werden Personen- oder Gruppenwerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="d1484-174">This column stores Person or Group values.</span></span>
| <span data-ttu-id="d1484-175">**text**</span><span class="sxs-lookup"><span data-stu-id="d1484-175">**text**</span></span>          | <span data-ttu-id="d1484-176">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="d1484-176">[textColumn][]</span></span>          | <span data-ttu-id="d1484-177">In dieser Spalte werden Textwerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="d1484-177">This column stores text values.</span></span>

<span data-ttu-id="d1484-178">Hinweis: Diese Eigenschaften entsprechen der [SPFieldType][]-Enumeration von SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d1484-178">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="d1484-179">Während die am häufigsten verwendeten Feldtypen oben dargestellt werden, Fehlen dieser API noch einige.</span><span class="sxs-lookup"><span data-stu-id="d1484-179">While the most common field types are represented above, this API is still missing some.</span></span>
<span data-ttu-id="d1484-180">In diesen Fällen werden keine der Spaltentyp-Facets aufgefüllt und die Spalte weist nur die grundlegenden Eigenschaften auf.</span><span class="sxs-lookup"><span data-stu-id="d1484-180">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="d1484-181">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="d1484-181">Remarks</span></span>

<span data-ttu-id="d1484-182">ColumnDefinitions und Feldwerte für `hidden`-Spalten werden standardmäßig nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d1484-182">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="d1484-183">Um diese bei der Auflistung von **ColumnDefinitions** anzuzeigen, fügen Sie `hidden` in Ihre `$select`-Anweisung ein.</span><span class="sxs-lookup"><span data-stu-id="d1484-183">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="d1484-184">Um diese beim Anzeigen von **field**-Werten mit [listItems][listItem] anzuzeigen, fügen Sie die gewünschten Spalten ein, indem Sie `$select` in Ihre Anweisung aufnehmen.</span><span class="sxs-lookup"><span data-stu-id="d1484-184">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[Feldern]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

<span data-ttu-id="d1484-197">
  [SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span><span class="sxs-lookup"><span data-stu-id="d1484-197">[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
