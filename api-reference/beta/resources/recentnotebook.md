---
title: recentNotebook-Ressourcentyp
description: Ein OneNote-Notizbuch, auf das kürzlich zugegriffen wurde. Ein **recentNotebook** ist vergleichbar mit einem Notizbuch, hat jedoch weniger Eigenschaften.
ms.openlocfilehash: c3b717fcebdc229864aefe13c6452ce5eb95fc53
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061884"
---
# <a name="recentnotebook-resource-type"></a>recentNotebook-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ein OneNote-Notizbuch, auf das kürzlich zugegriffen wurde. Ein **recentNotebook** ist vergleichbar mit einem [Notizbuch](notebook.md), hat jedoch weniger Eigenschaften.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|name|String|Der Name des Notizbuchs.|
|lastAccessedTime|DateTimeOffset|Das Datum und die Uhrzeit der letzten Änderung des Notizbuchs. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.|
|Links|[recentNotebookLinks](recentnotebooklinks.md)|Links zum Öffnen des Notizbuchs. Der Link `oneNoteClientURL` öffnet das Notizbuch im OneNote-Client, sofern er installiert ist. Der Link `oneNoteWebURL` öffnet das Notizbuch in OneNote Online.|
|sourceService|Zeichenfolge|Der Back-End-Speicher, in dem das Notizbuch gespeichert ist (entweder `OneDriveForBusiness` oder `OneDrive`).|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebook"
}-->

```json
{
  "displayName": "String",
  "lastAccessedTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.recentNotebookLinks"},
  "sourceService": "String"
}

```

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[getRecentNotebooks](../api/notebook-getrecentnotebooks.md) | Sammlung [notebook](notebook.md) | Dient zum Abrufen einer Sammlung der zuletzt geöffneten Notizbücher des Benutzers. |