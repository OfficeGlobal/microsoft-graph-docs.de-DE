---
title: recentNotebook-Ressourcentyp
description: Ein OneNote-Notizbuch, auf das kürzlich zugegriffen wurde. Ein **recentNotebook** ist vergleichbar mit einem Notizbuch, hat jedoch weniger Eigenschaften.
localization_priority: Normal
ms.openlocfilehash: 67c707043e5b6ca65cd72ddc323b5a484f0f2959
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889222"
---
# <a name="recentnotebook-resource-type"></a>recentNotebook-Ressourcentyp

Ein OneNote-Notizbuch, auf das kürzlich zugegriffen wurde. Ein **recentNotebook** ist vergleichbar mit einem [Notizbuch](notebook.md), hat jedoch weniger Eigenschaften.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|displayName|Zeichenfolge|Der Name des Notizbuchs.|
|lastAccessedTime|DateTimeOffset|Das Datum und die Uhrzeit der letzten Änderung des Notizbuchs. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.|
|Links|[recentNotebookLinks](recentnotebooklinks.md)|Links zum Öffnen des Notizbuchs. Der Link `oneNoteClientURL` öffnet das Notizbuch im OneNote-Client, sofern er installiert ist. Der Link `oneNoteWebURL` öffnet das Notizbuch in OneNote Online.|
|sourceService|onenoteSourceService|Der Back-End-Speicher, in dem das Notizbuch gespeichert ist (entweder `OneDriveForBusiness` oder `OneDrive`).|

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
