---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
ms.openlocfilehash: f4e0c3002068ec7dc8ee280b8e8143af621f178c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528935"
---
# <a name="columndefinition-resource-type"></a>ColumnDefinition Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer Ressource ColumnDefinition.

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

## <a name="properties"></a>Eigenschaften

Spalten können verschiedene Datentypen enthalten.
Die folgenden Eigenschaften geben an, welche Arten von Daten in einer Spalte gespeichert werden sowie weitere Einstellungen für die Daten.
Die Typ-bezogene Eigenschaften (boolean, berechnet, Auswahl, Währung, DateTime, Suche, Anzahl, PersonOrGroup, Text) schließen sich gegenseitig aus – eine Spalte kann nur einer von ihnen angegeben haben.

| Eigenschaftenname           | Typ    | Beschreibung
|:------------------------|:--------|:-----------------------------------------
| **columnGroup**         | string  | Für Websitespalten der Name der Gruppe, zu der dieser Spalte gehört. Dadurch können dazugehörige Spalten einfacher organisiert werden.
| **description**         | string  | Für den Benutzer sichtbare Beschreibung der Spalte.
| **displayName**         | string  | Für den Benutzer sichtbarer Name der Spalte.
| **enforceUniqueValues** | Boolescher Wert | Wenn der Wert true ist, dürfen keine der Elemente für diese Spalte den gleichen Wert aufweisen.
| **hidden**              | Boolescher Wert | Gibt an, ob die Spalte auf der Benutzeroberfläche angezeigt wird.
| **id**                  | string  | Die eindeutige ID für die Spalte.
| **indexed**             | Boolescher Wert | Gibt an, ob die Spaltenwerte für das Sortieren und Suchen verwendet werden können.
| **name**                | string  | Der in der API sichtbare Name der Spalte, wie er in den  [Feldern][] eines [ListItem][] angezeigt wird. Weitere Informationen zum für den Benutzer sichtbaren Namen finden Sie unter **displayName**.
| **readOnly**            | bool    | Gibt an, ob die Werte in den Spalten geändert werden können.
| **required**            | boolean | Gibt an, ob die Werte in den Spalten obligatorisch sind.
| **boolean**       | [booleanColumn][]       | In dieser Spalte werden boolesche Werte gespeichert.
| **calculated**    | [calculatedColumn][]    | Die Daten in dieser Spalte werden anhand von anderen Spalten berechnet.
| **choice**        | [choiceColumn][]        | In dieser Spalte werden Daten aus einer Auswahlliste gespeichert.
| **currency**      | [currencyColumn][]      | In dieser Spalte sind die Währungswerte gespeichert.
| **dateTime**      | [dateTimeColumn][]      | In dieser Spalte sind die DateTime-Werte gespeichert.
| **defaultValue**  | [defaultColumnValue][]  | Der Standardwert für diese Spalte.
| Geolocation   | [geolocationColumn][]   | Diese Spalte speichert ein GeoLocation-Objekt.
| **lookup**        | [lookupColumn][]        | Die Daten in dieser Spalte werden aus einer anderen Quelle dieser Website abgerufen.
| **number**        | [numberColumn][]        | In dieser Spalte werden Zahlenwerte gespeichert.
| **personOrGroup** | [personOrGroupColumn][] | In dieser Spalte werden Personen- oder Gruppenwerte gespeichert.
| **text**          | [textColumn][]          | In dieser Spalte werden Textwerte gespeichert.

>Hinweis: Diese Eigenschaften entsprechen der **SPFieldType**-Enumeration von SharePoint.
Während die am häufigsten verwendeten Feldtypen in der vorherigen Tabelle dargestellt werden, ist dieses Beta API noch einige fehlt.
In diesen Fällen werden keine der Spaltentyp-Facets aufgefüllt und die Spalte weist nur die grundlegenden Eigenschaften auf.

## <a name="remarks"></a>Bemerkungen

ColumnDefinitions und Feldwerte für `hidden`-Spalten werden standardmäßig nicht angezeigt.
Um diese bei der Auflistung von **ColumnDefinitions** anzuzeigen, fügen Sie `hidden` in Ihre `$select`-Anweisung ein.
Um diese beim Anzeigen von **field**-Werten mit [listItems][listItem] anzuzeigen, fügen Sie die gewünschten Spalten ein, indem Sie `$select` in Ihre Anweisung aufnehmen.

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
[listItem]: listitem.md


  [SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx

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
