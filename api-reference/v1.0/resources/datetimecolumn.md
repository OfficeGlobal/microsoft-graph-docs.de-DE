---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
ms.openlocfilehash: 6f2c14d5fa67fa80c869c20081250bfa55e0f5e4
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267829"
---
# <a name="datetimecolumn-resource-type"></a>DateTimeColumn-Ressourcentyp

Die **dateTimeColumn** einer [columnDefinition](columnDefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Daten oder Uhrzeiten handelt.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **dateTimeColumn**-Ressource.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname      | Typ               | Beschreibung
|:-------------------|:-------------------|:----------------------------------------------
| **displayAs**      | Zeichenfolge             | Wie sollte der Wert in der UX dargestellt werden? Muss `default`, `friendly` oder `standard` sein. Weitere Einzelheiten finden Sie weiter unten. Wenn nicht angegeben, werden sie als `default` behandelt.
| **Format**         | Zeichenfolge             | Gibt an, ob der Wert nur als Datum oder als Datum und Uhrzeit angezeigt werden soll. Muss einer von `dateOnly` sein, oder `dateTime`

## <a name="displayas-options"></a>DisplayAs-Optionen

| Wert        | Beschreibung
|:-------------|:--------------------------------------------------------------
| **default**  | Verwendet das standardmäßige Rendering in der UX.
| **benutzerfreundlich** | Verwendet eine benutzerfreundliche relative Darstellung (z. B. "heute um 15:00 Uhr")
| **standard** | Verwendet die standardmäßige absolute Darstellung (z. B. "10.05.2017 15:20 Uhr")


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/datetimecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(default,friendly,standard) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/datetimecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(dateOnly,dateTime) are in resource, but () are in table"
  ],
  "tocPath": "Resources/DateTimeColumn"
} -->
