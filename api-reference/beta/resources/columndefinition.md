---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
ms.openlocfilehash: ddd6b3c6d3048bf7a6d3ab2dbc8ff7259651ee2f
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481160"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="3b2a9-102">columnDefinition-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3b2a9-102">columnDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="3b2a9-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3b2a9-103">JSON representation</span></span>

<span data-ttu-id="3b2a9-104">Es folgt eine JSON-Darstellung einer columnDefinition-Ressource.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-104">Here is a JSON representation of a columnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3b2a9-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3b2a9-105">Properties</span></span>

<span data-ttu-id="3b2a9-106">Spalten können verschiedene Datentypen enthalten.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-106">Columns can hold data of various types.</span></span>
<span data-ttu-id="3b2a9-107">Die folgenden Eigenschaften geben an, welche Arten von Daten in einer Spalte gespeichert werden sowie weitere Einstellungen für die Daten.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-107">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="3b2a9-108">Die typbezogenen Eigenschaften (Boolean, Calculated, Choice, Currency, dateTime, Lookup, Number, personOrGroup, Text) schließen sich gegenseitig aus – eine Spalte kann nur eine von Ihnen angeben.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-108">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="3b2a9-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="3b2a9-109">Property name</span></span>           | <span data-ttu-id="3b2a9-110">Typ</span><span class="sxs-lookup"><span data-stu-id="3b2a9-110">Type</span></span>    | <span data-ttu-id="3b2a9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b2a9-111">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="3b2a9-112">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-112">**columnGroup**</span></span>         | <span data-ttu-id="3b2a9-113">string</span><span class="sxs-lookup"><span data-stu-id="3b2a9-113">string</span></span>  | <span data-ttu-id="3b2a9-114">Für Websitespalten der Name der Gruppe, zu der dieser Spalte gehört.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-114">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="3b2a9-115">Dadurch können dazugehörige Spalten einfacher organisiert werden.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-115">Helps organize related columns.</span></span>
| <span data-ttu-id="3b2a9-116">**description**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-116">**description**</span></span>         | <span data-ttu-id="3b2a9-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3b2a9-117">string</span></span>  | <span data-ttu-id="3b2a9-118">Für den Benutzer sichtbare Beschreibung der Spalte.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-118">The user-facing description of the column.</span></span>
| <span data-ttu-id="3b2a9-119">**displayName**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-119">**displayName**</span></span>         | <span data-ttu-id="3b2a9-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3b2a9-120">string</span></span>  | <span data-ttu-id="3b2a9-121">Für den Benutzer sichtbarer Name der Spalte.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-121">The user-facing name of the column.</span></span>
| <span data-ttu-id="3b2a9-122">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-122">**enforceUniqueValues**</span></span> | <span data-ttu-id="3b2a9-123">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3b2a9-123">boolean</span></span> | <span data-ttu-id="3b2a9-124">Wenn der Wert true ist, dürfen keine der Elemente für diese Spalte den gleichen Wert aufweisen.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-124">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="3b2a9-125">**hidden**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-125">**hidden**</span></span>              | <span data-ttu-id="3b2a9-126">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3b2a9-126">boolean</span></span> | <span data-ttu-id="3b2a9-127">Gibt an, ob die Spalte auf der Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-127">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="3b2a9-128">**id**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-128">**id**</span></span>                  | <span data-ttu-id="3b2a9-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3b2a9-129">string</span></span>  | <span data-ttu-id="3b2a9-130">Die eindeutige ID für die Spalte.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-130">The unique identifier for the column.</span></span>
| <span data-ttu-id="3b2a9-131">**indexed**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-131">**indexed**</span></span>             | <span data-ttu-id="3b2a9-132">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3b2a9-132">boolean</span></span> | <span data-ttu-id="3b2a9-133">Gibt an, ob die Spaltenwerte für das Sortieren und Suchen verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-133">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="3b2a9-134">**name**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-134">**name**</span></span>                | <span data-ttu-id="3b2a9-135">string</span><span class="sxs-lookup"><span data-stu-id="3b2a9-135">string</span></span>  | <span data-ttu-id="3b2a9-136">Der in der API sichtbare Name der Spalte, wie er in den  [Feldern][] eines [ListItem][] angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-136">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="3b2a9-137">Weitere Informationen zum für den Benutzer sichtbaren Namen finden Sie unter **displayName**.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-137">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="3b2a9-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-138">**readOnly**</span></span>            | <span data-ttu-id="3b2a9-139">bool</span><span class="sxs-lookup"><span data-stu-id="3b2a9-139">bool</span></span>    | <span data-ttu-id="3b2a9-140">Gibt an, ob die Werte in den Spalten geändert werden können.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-140">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="3b2a9-141">**required**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-141">**required**</span></span>            | <span data-ttu-id="3b2a9-142">boolean</span><span class="sxs-lookup"><span data-stu-id="3b2a9-142">boolean</span></span> | <span data-ttu-id="3b2a9-143">Gibt an, ob die Werte in den Spalten obligatorisch sind.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-143">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="3b2a9-144">**boolean**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-144">**boolean**</span></span>       | <span data-ttu-id="3b2a9-145">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="3b2a9-145">[booleanColumn][]</span></span>       | <span data-ttu-id="3b2a9-146">In dieser Spalte werden boolesche Werte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-146">This column stores boolean values.</span></span>
| <span data-ttu-id="3b2a9-147">**calculated**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-147">**calculated**</span></span>    | <span data-ttu-id="3b2a9-148">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="3b2a9-148">[calculatedColumn][]</span></span>    | <span data-ttu-id="3b2a9-149">Die Daten in dieser Spalte werden anhand von anderen Spalten berechnet.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-149">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="3b2a9-150">**choice**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-150">**choice**</span></span>        | <span data-ttu-id="3b2a9-151">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="3b2a9-151">[choiceColumn][]</span></span>        | <span data-ttu-id="3b2a9-152">In dieser Spalte werden Daten aus einer Auswahlliste gespeichert.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-152">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="3b2a9-153">**currency**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-153">**currency**</span></span>      | <span data-ttu-id="3b2a9-154">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="3b2a9-154">[currencyColumn][]</span></span>      | <span data-ttu-id="3b2a9-155">In dieser Spalte sind die Währungswerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-155">This column stores currency values.</span></span>
| <span data-ttu-id="3b2a9-156">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-156">**dateTime**</span></span>      | <span data-ttu-id="3b2a9-157">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="3b2a9-157">[dateTimeColumn][]</span></span>      | <span data-ttu-id="3b2a9-158">In dieser Spalte sind die DateTime-Werte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-158">This column stores DateTime values.</span></span>
| <span data-ttu-id="3b2a9-159">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-159">**defaultValue**</span></span>  | <span data-ttu-id="3b2a9-160">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="3b2a9-160">[defaultColumnValue][]</span></span>  | <span data-ttu-id="3b2a9-161">Der Standardwert für diese Spalte.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-161">The default value for this column.</span></span>
| <span data-ttu-id="3b2a9-162">**Geolocation**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-162">**geolocation**</span></span>   | <span data-ttu-id="3b2a9-163">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="3b2a9-163">[geolocationColumn][]</span></span>   | <span data-ttu-id="3b2a9-164">In dieser Spalte wird ein Geolocation-Speicher gespeichert.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-164">This column stores a geolocation.</span></span>
| <span data-ttu-id="3b2a9-165">**lookup**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-165">**lookup**</span></span>        | <span data-ttu-id="3b2a9-166">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="3b2a9-166">[lookupColumn][]</span></span>        | <span data-ttu-id="3b2a9-167">Die Daten in dieser Spalte werden aus einer anderen Quelle dieser Website abgerufen.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-167">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="3b2a9-168">**number**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-168">**number**</span></span>        | <span data-ttu-id="3b2a9-169">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="3b2a9-169">[numberColumn][]</span></span>        | <span data-ttu-id="3b2a9-170">In dieser Spalte werden Zahlenwerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-170">This column stores number values.</span></span>
| <span data-ttu-id="3b2a9-171">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-171">**personOrGroup**</span></span> | <span data-ttu-id="3b2a9-172">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="3b2a9-172">[personOrGroupColumn][]</span></span> | <span data-ttu-id="3b2a9-173">In dieser Spalte werden Personen- oder Gruppenwerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-173">This column stores Person or Group values.</span></span>
| <span data-ttu-id="3b2a9-174">**text**</span><span class="sxs-lookup"><span data-stu-id="3b2a9-174">**text**</span></span>          | <span data-ttu-id="3b2a9-175">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="3b2a9-175">[textColumn][]</span></span>          | <span data-ttu-id="3b2a9-176">In dieser Spalte werden Textwerte gespeichert.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-176">This column stores text values.</span></span>

><span data-ttu-id="3b2a9-177">**Hinweis:** Diese Eigenschaften entsprechen der FieldType [][] -Enumeration von SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-177">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="3b2a9-178">Während die am häufigsten verwendeten Feldtypen in der vorherigen Tabelle dargestellt werden, Fehlen dieser Beta-API noch einige.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-178">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="3b2a9-179">In diesen Fällen werden keine der Spaltentyp-Facets aufgefüllt und die Spalte weist nur die grundlegenden Eigenschaften auf.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-179">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="3b2a9-180">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="3b2a9-180">Remarks</span></span>

<span data-ttu-id="3b2a9-181">ColumnDefinitions und Feldwerte für `hidden`-Spalten werden standardmäßig nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-181">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="3b2a9-182">Um diese bei der Auflistung von **ColumnDefinitions** anzuzeigen, fügen Sie `hidden` in Ihre `$select`-Anweisung ein.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-182">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="3b2a9-183">Um diese beim Anzeigen von **field**-Werten mit [listItems][listItem] anzuzeigen, fügen Sie die gewünschten Spalten ein, indem Sie `$select` in Ihre Anweisung aufnehmen.</span><span class="sxs-lookup"><span data-stu-id="3b2a9-183">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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
[Feldern]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

<span data-ttu-id="3b2a9-197">
  [SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span><span class="sxs-lookup"><span data-stu-id="3b2a9-197">[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition",
  "suppressions": [
    "Error: /api-reference/beta/resources/columndefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
