---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: 2fd6c08e1cfc28a77019d174763b9d698519b6a2
ms.sourcegitcommit: 9e4dc7745eb1bbbe595afd8c7f3db4c19c6bb4ac
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/29/2018
ms.locfileid: "23271315"
---
# <a name="columndefinition-resource"></a>ColumnDefinition-Ressource

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer ColumnDefinition-Ressource.

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

## <a name="properties"></a>Eigenschaften

Die **ColumnDefinition**-Ressource weist folgende Eigenschaften auf.

| Eigenschaftenname           | Typ    | Beschreibung
|:------------------------|:--------|:-----------------------------------------
| **columnGroup**         | Zeichenfolge  | Für Websitespalten der Name der Gruppe, zu der dieser Spalte gehört. Dadurch können dazugehörige Spalten einfacher organisiert werden.
| **description**         | Zeichenfolge  | Für den Benutzer sichtbare Beschreibung der Spalte.
| **displayName**         | Zeichenfolge  | Für den Benutzer sichtbarer Name der Spalte.
| **enforceUniqueValues** | Boolescher Wert | Wenn der Wert true ist, dürfen keine der Elemente für diese Spalte den gleichen Wert aufweisen.
| **ausgeblendet**              | Boolescher Wert | Gibt an, ob die Spalte auf der Benutzeroberfläche angezeigt wird.
| **ID**                  | Zeichenfolge  | Die eindeutige ID für die Spalte.
| **indiziert**             | Boolescher Wert | Gibt an, ob die Spaltenwerte für das Sortieren und Suchen verwendet werden können.
| **Name**                | Zeichenfolge  | Der in der API sichtbare Name der Spalte, wie er in den  [Feldern][] eines [ListItem][] angezeigt wird. Weitere Informationen zum für den Benutzer sichtbaren Namen finden Sie unter **displayName**.
| **schreibgeschützt**            | Boolescher Wert    | Gibt an, ob die Werte in den Spalten geändert werden können.
| **erforderlich**            | Boolescher Wert | Gibt an, ob die Werte in den Spalten obligatorisch sind.

Spalten können verschiedene Datentypen enthalten.
Die folgenden Eigenschaften geben an, welche Arten von Daten in einer Spalte gespeichert werden sowie weitere Einstellungen für die Daten.
Diese Eigenschaften schließen sich gegenseitig aus – in einer Spalte kann nur eines der beiden angegeben werden.

| Eigenschaftenname     | Typ                    | Beschreibung
|:------------------|:------------------------|:-------------------------------
| **Boolescher Wert**       | [booleanColumn][]       | In dieser Spalte werden boolesche Werte gespeichert.
| **berechnet**    | [calculatedColumn][]    | Die Daten in dieser Spalte werden anhand von anderen Spalten berechnet.
| **Auswahl**        | [choiceColumn][]        | In dieser Spalte werden Daten aus einer Auswahlliste gespeichert.
| **Währung**      | [currencyColumn][]      | In dieser Spalte sind die Währungswerte gespeichert.
| **dateTime**      | [dateTimeColumn][]      | In dieser Spalte sind die DateTime-Werte gespeichert.
| **defaultValue**  | [defaultColumnValue][]  | Der Standardwert für diese Spalte.
| **auflisten**        | [lookupColumn][]        | Die Daten in dieser Spalte werden aus einer anderen Quelle dieser Website abgerufen.
| **Zahl**        | [numberColumn][]        | In dieser Spalte werden Zahlenwerte gespeichert.
| **personOrGroup** | [personOrGroupColumn][] | In dieser Spalte werden Personen- oder Gruppenwerte gespeichert.
| **SMS**          | [textColumn][]          | In dieser Spalte werden Textwerte gespeichert.

Hinweis: Diese Eigenschaften entsprechen der [SPFieldType][]-Enumeration von SharePoint.
Obwohl die meisten gängigen Feldtypen vorstehend dargestellt sind, fehlen bei dieser API noch einige.
In diesen Fällen werden keine der Spaltentyp-Facets aufgefüllt und die Spalte weist nur die grundlegenden Eigenschaften auf.

## <a name="remarks"></a>Bemerkungen

ColumnDefinitions und Feldwerte für `hidden`-Spalten werden standardmäßig nicht angezeigt.
Um diese bei der Auflistung von **ColumnDefinitions** anzuzeigen, fügen Sie `hidden` in Ihre `$select`-Anweisung ein.
Um diese beim Anzeigen von **field**-Werten mit [listItems][listItem] anzuzeigen, fügen Sie die gewünschten Spalten ein, indem Sie `$select` in Ihre Anweisung aufnehmen.

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
[Datenfelder]: fieldvalueset.md
[listItem]: listitem.md

[SPFieldType]: https://msdn.microsoft.com/en-us/library/microsoft.sharepoint.spfieldtype.aspx

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
