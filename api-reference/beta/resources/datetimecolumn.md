---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
ms.openlocfilehash: da8fe44e377a071ee3f20b82f7190b690dcfd6b2
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482168"
---
# <a name="datetimecolumn-resource-type"></a>DateTimeColumn-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **dateTimeColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Daten oder Uhrzeiten handelt.

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
| **format**         | string             | Gibt an, ob der Wert nur als Datum oder als Datum und Uhrzeit angezeigt werden soll. Muss `dateOnly` oder `dateTime` sein.

## <a name="displayas-values"></a>DisplayAs-Werte

| Wert        | Beschreibung
|:-------------|:--------------------------------------------------------------
| **default**  | Verwendet das standardmäßige Rendering in der UX.
| **friendly** | Verwendet eine benutzerfreundliche relative Darstellung (z. B. "heute um 15:00 Uhr")
| **standard** | Verwendet die standardmäßige absolute Darstellung (z. B. "10.05.2017 15:20 Uhr")


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/datetimecolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
