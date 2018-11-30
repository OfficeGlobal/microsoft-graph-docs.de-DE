---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: 96587cc1b3badf2d5fcc90bc7c1d2b1cfb710f6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016885"
---
# <a name="columndefinition-resource"></a><span data-ttu-id="e8689-102">ColumnDefinition-Ressource</span><span class="sxs-lookup"><span data-stu-id="e8689-102">ColumnDefinition resource</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8689-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e8689-103">JSON representation</span></span>

<span data-ttu-id="e8689-104">Es folgt eine JSON-Darstellung einer ColumnDefinition-Ressource.</span><span class="sxs-lookup"><span data-stu-id="e8689-104">Here is a JSON representation of a ColumnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="e8689-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e8689-105">Properties</span></span>

<span data-ttu-id="e8689-106">Die **ColumnDefinition**-Ressource weist folgende Eigenschaften auf.</span><span class="sxs-lookup"><span data-stu-id="e8689-106">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="e8689-107">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="e8689-107">Property name</span></span>           | <span data-ttu-id="e8689-108">Typ</span><span class="sxs-lookup"><span data-stu-id="e8689-108">Type</span></span>    | <span data-ttu-id="e8689-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8689-109">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="e8689-110">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="e8689-110">**columnGroup**</span></span>         | <span data-ttu-id="e8689-111">string</span><span class="sxs-lookup"><span data-stu-id="e8689-111">string</span></span>  | <span data-ttu-id="e8689-112">Für Websitespalten der Name der Gruppe, zu der dieser Spalte gehört.</span><span class="sxs-lookup"><span data-stu-id="e8689-112">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="e8689-113">Dadurch können dazugehörige Spalten einfacher organisiert werden.</span><span class="sxs-lookup"><span data-stu-id="e8689-113">Helps organize related columns.</span></span>
| <span data-ttu-id="e8689-114">**description**</span><span class="sxs-lookup"><span data-stu-id="e8689-114">**description**</span></span>         | <span data-ttu-id="e8689-115">string</span><span class="sxs-lookup"><span data-stu-id="e8689-115">string</span></span>  | <span data-ttu-id="e8689-116">Für den Benutzer sichtbare Beschreibung der Spalte.</span><span class="sxs-lookup"><span data-stu-id="e8689-116">The user-facing description of the column.</span></span>
| <span data-ttu-id="e8689-117">**displayName**</span><span class="sxs-lookup"><span data-stu-id="e8689-117">**displayName**</span></span>         | <span data-ttu-id="e8689-118">string</span><span class="sxs-lookup"><span data-stu-id="e8689-118">string</span></span>  | <span data-ttu-id="e8689-119">Für den Benutzer sichtbarer Name der Spalte.</span><span class="sxs-lookup"><span data-stu-id="e8689-119">The user-facing name of the column.</span></span>
| <span data-ttu-id="e8689-120">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="e8689-120">**enforceUniqueValues**</span></span> | <span data-ttu-id="e8689-121">boolean</span><span class="sxs-lookup"><span data-stu-id="e8689-121">boolean</span></span> | <span data-ttu-id="e8689-122">Wenn der Wert true ist, dürfen keine der Elemente für diese Spalte den gleichen Wert aufweisen.</span><span class="sxs-lookup"><span data-stu-id="e8689-122">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="e8689-123">**hidden**</span><span class="sxs-lookup"><span data-stu-id="e8689-123">**hidden**</span></span>              | <span data-ttu-id="e8689-124">boolean</span><span class="sxs-lookup"><span data-stu-id="e8689-124">boolean</span></span> | <span data-ttu-id="e8689-125">Gibt an, ob die Spalte auf der Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e8689-125">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="e8689-126">**id**</span><span class="sxs-lookup"><span data-stu-id="e8689-126">**id**</span></span>                  | <span data-ttu-id="e8689-127">string</span><span class="sxs-lookup"><span data-stu-id="e8689-127">string</span></span>  | <span data-ttu-id="e8689-128">Die eindeutige ID für die Spalte.</span><span class="sxs-lookup"><span data-stu-id="e8689-128">The unique identifier for the column.</span></span>
| <span data-ttu-id="e8689-129">**indexed**</span><span class="sxs-lookup"><span data-stu-id="e8689-129">**indexed**</span></span>             | <span data-ttu-id="e8689-130">boolean</span><span class="sxs-lookup"><span data-stu-id="e8689-130">boolean</span></span> | <span data-ttu-id="e8689-131">Gibt an, ob die Spaltenwerte für das Sortieren und Suchen verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="e8689-131">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="e8689-132">**name**</span><span class="sxs-lookup"><span data-stu-id="e8689-132">**name**</span></span>                | <span data-ttu-id="e8689-133">string</span><span class="sxs-lookup"><span data-stu-id="e8689-133">string</span></span>  | <span data-ttu-id="e8689-134">Der in der API sichtbare Name der Spalte, wie er in den  [Feldern][] eines [ListItem][] angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e8689-134">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="e8689-135">Weitere Informationen zum für den Benutzer sichtbaren Namen finden Sie unter **displayName**.</span><span class="sxs-lookup"><span data-stu-id="e8689-135">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="e8689-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="e8689-136">**readOnly**</span></span>            | <span data-ttu-id="e8689-137">bool</span><span class="sxs-lookup"><span data-stu-id="e8689-137">bool</span></span>    | <span data-ttu-id="e8689-138">Gibt an, ob die Werte in den Spalten geändert werden können.</span><span class="sxs-lookup"><span data-stu-id="e8689-138">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="e8689-139">**required**</span><span class="sxs-lookup"><span data-stu-id="e8689-139">**required**</span></span>            | <span data-ttu-id="e8689-140">boolean</span><span class="sxs-lookup"><span data-stu-id="e8689-140">boolean</span></span> | <span data-ttu-id="e8689-141">Gibt an, ob die Werte in den Spalten obligatorisch sind.</span><span class="sxs-lookup"><span data-stu-id="e8689-141">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="e8689-142">Spalten können verschiedene Datentypen enthalten.</span><span class="sxs-lookup"><span data-stu-id="e8689-142">Columns can hold data of various types.</span></span>
<span data-ttu-id="e8689-143">Die folgenden Eigenschaften geben an, welche Arten von Daten in einer Spalte gespeichert werden sowie weitere Einstellungen für die Daten.</span><span class="sxs-lookup"><span data-stu-id="e8689-143">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="e8689-144">Diese Eigenschaften schließen sich gegenseitig aus – in einer Spalte kann nur eines der beiden angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="e8689-144">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="e8689-145">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="e8689-145">Property name</span></span>     | <span data-ttu-id="e8689-146">Typ</span><span class="sxs-lookup"><span data-stu-id="e8689-146">Type</span></span>                    | <span data-ttu-id="e8689-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8689-147">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="e8689-148">**boolean**</span><span class="sxs-lookup"><span data-stu-id="e8689-148">**boolean**</span></span>       | <span data-ttu-id="e8689-149">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="e8689-149">[booleanColumn][]</span></span>       | <span data-ttu-id="e8689-150">In dieser Spalte werden boolesche Werte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="e8689-150">This column stores boolean values.</span></span>
| <span data-ttu-id="e8689-151">**calculated**</span><span class="sxs-lookup"><span data-stu-id="e8689-151">**calculated**</span></span>    | <span data-ttu-id="e8689-152">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="e8689-152">[calculatedColumn][]</span></span>    | <span data-ttu-id="e8689-153">Die Daten in dieser Spalte werden anhand von anderen Spalten berechnet.</span><span class="sxs-lookup"><span data-stu-id="e8689-153">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="e8689-154">**choice**</span><span class="sxs-lookup"><span data-stu-id="e8689-154">**choice**</span></span>        | <span data-ttu-id="e8689-155">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="e8689-155">[choiceColumn][]</span></span>        | <span data-ttu-id="e8689-156">In dieser Spalte werden Daten aus einer Auswahlliste gespeichert.</span><span class="sxs-lookup"><span data-stu-id="e8689-156">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="e8689-157">**currency**</span><span class="sxs-lookup"><span data-stu-id="e8689-157">**currency**</span></span>      | <span data-ttu-id="e8689-158">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="e8689-158">[currencyColumn][]</span></span>      | <span data-ttu-id="e8689-159">In dieser Spalte sind die Währungswerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="e8689-159">This column stores currency values.</span></span>
| <span data-ttu-id="e8689-160">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="e8689-160">**dateTime**</span></span>      | <span data-ttu-id="e8689-161">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="e8689-161">[dateTimeColumn][]</span></span>      | <span data-ttu-id="e8689-162">In dieser Spalte sind die DateTime-Werte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="e8689-162">This column stores DateTime values.</span></span>
| <span data-ttu-id="e8689-163">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="e8689-163">**defaultValue**</span></span>  | <span data-ttu-id="e8689-164">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="e8689-164">[defaultColumnValue][]</span></span>  | <span data-ttu-id="e8689-165">Der Standardwert für diese Spalte.</span><span class="sxs-lookup"><span data-stu-id="e8689-165">The default value for this column.</span></span>
| <span data-ttu-id="e8689-166">**lookup**</span><span class="sxs-lookup"><span data-stu-id="e8689-166">**lookup**</span></span>        | <span data-ttu-id="e8689-167">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="e8689-167">[lookupColumn][]</span></span>        | <span data-ttu-id="e8689-168">Die Daten in dieser Spalte werden aus einer anderen Quelle dieser Website abgerufen.</span><span class="sxs-lookup"><span data-stu-id="e8689-168">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="e8689-169">**number**</span><span class="sxs-lookup"><span data-stu-id="e8689-169">**number**</span></span>        | <span data-ttu-id="e8689-170">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="e8689-170">[numberColumn][]</span></span>        | <span data-ttu-id="e8689-171">In dieser Spalte werden Zahlenwerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="e8689-171">This column stores number values.</span></span>
| <span data-ttu-id="e8689-172">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="e8689-172">**personOrGroup**</span></span> | <span data-ttu-id="e8689-173">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="e8689-173">[personOrGroupColumn][]</span></span> | <span data-ttu-id="e8689-174">In dieser Spalte werden Personen- oder Gruppenwerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="e8689-174">This column stores Person or Group values.</span></span>
| <span data-ttu-id="e8689-175">**text**</span><span class="sxs-lookup"><span data-stu-id="e8689-175">**text**</span></span>          | <span data-ttu-id="e8689-176">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="e8689-176">[textColumn][]</span></span>          | <span data-ttu-id="e8689-177">In dieser Spalte werden Textwerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="e8689-177">This column stores text values.</span></span>

<span data-ttu-id="e8689-178">Hinweis: Diese Eigenschaften entsprechen der [SPFieldType][]-Enumeration von SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e8689-178">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="e8689-179">Während die am häufigsten verwendeten Feldtypen oben dargestellt werden, ist diese API immer noch einige nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e8689-179">While the most common field types are represented above, this API is still missing some.</span></span>
<span data-ttu-id="e8689-180">In diesen Fällen werden keine der Spaltentyp-Facets aufgefüllt und die Spalte weist nur die grundlegenden Eigenschaften auf.</span><span class="sxs-lookup"><span data-stu-id="e8689-180">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="e8689-181">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="e8689-181">Remarks</span></span>

<span data-ttu-id="e8689-182">ColumnDefinitions und Feldwerte für `hidden`-Spalten werden standardmäßig nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e8689-182">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="e8689-183">Um diese bei der Auflistung von **ColumnDefinitions** anzuzeigen, fügen Sie `hidden` in Ihre `$select`-Anweisung ein.</span><span class="sxs-lookup"><span data-stu-id="e8689-183">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="e8689-184">Um diese beim Anzeigen von **field**-Werten mit [listItems][listItem] anzuzeigen, fügen Sie die gewünschten Spalten ein, indem Sie `$select` in Ihre Anweisung aufnehmen.</span><span class="sxs-lookup"><span data-stu-id="e8689-184">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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

<span data-ttu-id="e8689-197">
  [SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span><span class="sxs-lookup"><span data-stu-id="e8689-197">[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
