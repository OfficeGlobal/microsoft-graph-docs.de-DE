---
title: page-Ressourcentyp
description: Eine Seite in einem OneNote-Notizbuch.
localization_priority: Normal
ms.openlocfilehash: b7c92aaae401e022a79f7c3b72cb15b3093d0b7d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879709"
---
# <a name="page-resource-type"></a>page-Ressourcentyp

Eine Seite in einem OneNote-Notizbuch.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenotePage"
}-->

```json
{
  "content": "stream",
  "contentUrl": "string",
  "createdByAppId": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "level": 1024,
  "links": {"@odata.type": "microsoft.graph.pageLinks"},
  "order": 1024,
  "self": "string",
  "title": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Inhalt|Stream|Der HTML-Inhalt der Seite.|
|contentUrl|Zeichenfolge|Die URL für die HTML-Inhalt der Seite.  Schreibgeschützt.|
|createdByAppId|Zeichenfolge|Der eindeutige Bezeichner der Anwendung, mit der die Seite erstellt wurde. Schreibgeschützt.|
|createdDateTime|DateTimeOffset|Das Datum und die Uhrzeit der Erstellung der Seite. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.|
|id|Zeichenfolge|Der eindeutige Bezeichner der Seite.  Schreibgeschützt.|
|lastModifiedDateTime|DateTimeOffset|Das Datum und die Uhrzeit der letzten Änderung der Seite. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.|
|Ebene|Int32|Die Einzugsebene der Seite. Schreibgeschützt.|
|links|[PageLinks](pagelinks.md)|Links zum Öffnen der Seite. Der Link `oneNoteClientURL` öffnet die Seite im systemeigenen OneNote-Client, sofern er installiert ist. Der Link `oneNoteWebUrl` öffnet die Seite in OneNote Online. Schreibgeschützt.|
|order|Int32|Die Anordnung der Seite im übergeordneten Abschnitt. Schreibgeschützt.|
|self|Zeichenfolge|Der Endpunkt, an dem Sie Details zur Seite abrufen können. Schreibgeschützt.|
|title|String|Der Titel der Seite. |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|parentNotebook|[Notebook](notebook.md)|Das Notizbuch, das die Seite enthält.  Schreibgeschützt.|
|parentSection|[OnenoteSection](section.md)|Der Abschnitt, der die Seite enthält. Schreibgeschützt.|

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Seite abrufen](../api/page-get.md) | [Page](page.md) |Dient zum Lesen der Eigenschaften und Beziehungen der Seite.|
|[Seiteninhalt aktualisieren](../api/page-update.md) | Keine |Dient zum Aktualisieren des HTML-Inhalts der Seite. |
|[Seite löschen](../api/page-delete.md) | Keine |Dient zum Löschen der Seite. |
|[copyToSection](../api/page-copytosection.md)| Keine |Kopiert die Seite in einen bestimmten Abschnitt.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
