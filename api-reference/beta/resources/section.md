---
title: section-Ressourcentyp
description: Ein Abschnitt in einem OneNote-Notizbuch. Abschnitte können Seiten enthalten.
localization_priority: Normal
ms.openlocfilehash: ea33cfae128a7ea796f3f14bd165210cbfec121d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574138"
---
# <a name="section-resource-type"></a>section-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein Abschnitt in einem OneNote-Notizbuch. Abschnitte können Seiten enthalten.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "@odata.type": "microsoft.graph.onenoteSection"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.sectionLinks"},
  "displayName": "string",
  "pagesUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.|
|createdDateTime|DateTimeOffset|Das Datum und die Uhrzeit der Erstellung des Abschnitts. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.|
|id|String|Der eindeutige Bezeichner des Abschnitts.  Schreibgeschützt.|
|isDefault|Boolean|Gibt an, ob dies der Standardabschnitt des Benutzers ist. Schreibgeschützt.|
|lastModifiedBy|[identitySet](identityset.md)|Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.|
|lastModifiedDateTime|DateTimeOffset|Das Datum und die Uhrzeit der letzten Änderung des Abschnitts. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.|
|links|[sectionLinks](sectionlinks.md)|Links zum Öffnen des Abschnitts. Der Link `oneNoteClientURL` öffnet den Abschnitt im systemeigenen OneNote-Client, sofern er installiert ist. Der Link `oneNoteWebURL` öffnet den Abschnitt in OneNote Online.|
|displayName|String|Der Name des Abschnitts. |
|pagesUrl|String|Der Endpunkt `pages`, an dem Sie Details für alle Seiten im Abschnitt abrufen können. Schreibgeschützt.|
|self|String|Der Endpunkt, an dem Sie Details zum Abschnitt abrufen können. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|pages|[OnenotePage](onenotepage.md) -Auflistung|Ruft die Sammlung von Seiten in dem Abschnitt ab.  Schreibgeschützt. Lässt Nullwerte zu.|
|parentNotebook|[Notizbuch](notebook.md)|Das Notizbuch, das den Abschnitt enthält.  Schreibgeschützt.|
|parentSectionGroup|[sectionGroup](sectiongroup.md)|Die Abschnittsgruppe, die den Abschnitt enthält.  Schreibgeschützt.|

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abschnitt abrufen](../api/section-get.md) | [onenoteSection](section.md) |Dient zum Lesen der Eigenschaften und Beziehungen des Abschnitts.|
|[Seite erstellen](../api/section-post-pages.md) |[onenotePage](onenotepage.md)| Dient zum Erstellen einer Seite durch Veröffentlichung in der pages-Sammlung im angegebenen Abschnitt.|
|[Seiten auflisten](../api/section-list-pages.md) |[OnenotePage](onenotepage.md) -Auflistung| Dient zum Abrufen einer Sammlung von Seiten im angegebenen Abschnitt.|
|[copyToNotebook](../api/section-copytonotebook.md)|Keine|Dient zum Kopieren des Abschnitts in ein bestimmtes Notizbuch.|
|[copyToSectionGroup](../api/section-copytosectiongroup.md)|Keine|Dient zum Kopieren des Abschnitts in eine bestimmte Abschnittsgruppe.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/section.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
