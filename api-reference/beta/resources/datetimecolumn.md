---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
ms.openlocfilehash: 9854ad35c602ff474604f2ca88e7182c325e797d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058863"
---
# <a name="datetimecolumn-resource-type"></a>DateTimeColumn-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
| **displayAs**      | string             | Wie sollte der Wert in der UX dargestellt werden? Muss `default`, `friendly` oder `standard` sein. Weitere Einzelheiten finden Sie weiter unten. Wenn nicht angegeben, werden sie als `default` behandelt.
| **format**         | string             | Gibt an, ob der Wert nur als Datum oder als Datum und Uhrzeit angezeigt werden soll. Muss `dateOnly` oder `dateTime` sein.

## <a name="displayas-values"></a>DisplayAs-Werte

| Wert        | Beschreibung
|:-------------|:--------------------------------------------------------------
| **default**  | Verwendet das standardmäßige Rendering in der UX.
| **friendly** | Verwendet eine benutzerfreundliche relative Darstellung (z. B. "heute um 15:00 Uhr")
| **standard** | Verwendet die standardmäßige absolute Darstellung (z. B. "10.05.2017 15:20 Uhr")


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn"
} -->
