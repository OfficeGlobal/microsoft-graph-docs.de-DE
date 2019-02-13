---
title: notebook-Ressourcentyp
description: Stellt ein OneNote-Notizbuch dar.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 96be6a41424260610794f9a0df4ef8e35dc1597f
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967333"
---
# <a name="notebook-resource-type"></a>notebook-Ressourcentyp

Stellt ein OneNote-Notizbuch dar.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.notebook"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "isShared": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.notebookLinks"},
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string",
  "userRole": "String"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.|
|createdDateTime|DateTimeOffset|Das Datum und die Uhrzeit der Erstellung des Notizbuchs. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.|
|id|string|Der eindeutige Bezeichner des Notizbuchs. Schreibgeschützt.|
|isDefault|Boolean|Gibt an, ob dies das Standardnotizbuch des Benutzers ist. Schreibgeschützt.|
|isShared|Boolean|Gibt an, ob das Notizbuch freigegeben ist. Wenn „true“, können auch andere Personen als der Besitzer den Inhalt des Notizbuchs sehen. Schreibgeschützt.|
|lastModifiedBy|[identitySet](identityset.md)|Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.|
|lastModifiedDateTime|DateTimeOffset|Das Datum und die Uhrzeit der letzten Änderung des Notizbuchs. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.|
|links|[NotebookLinks](notebooklinks.md)|Links zum Öffnen des Notizbuchs. Der Link `oneNoteClientURL` öffnet das Notizbuch im systemeigenen OneNote-Client, sofern er installiert ist. Der Link `oneNoteWebURL` öffnet das Notizbuch in OneNote Online.|
|displayName|Zeichenfolge|Der Name des Notizbuchs.|
|sectionGroupsUrl|Zeichenfolge|Die URL für die Navigationseigenschaft `sectionGroups`, die alle Abschnittsgruppen im Notizbuch zurückgibt. Schreibgeschützt.|
|sectionsUrl|Zeichenfolge|Die URL für die Navigationseigenschaft `sections`, die alle Abschnitte im Notizbuch zurückgibt. Schreibgeschützt.|
|self|String|Der Endpunkt, an dem Sie Details zum Notizbuch abrufen können. Schreibgeschützt.|
|userRole|onenoteUserRole|Mögliche Werte: `Owner`, `Contributor`, `Reader`, `None`. „Owner“ stellt Zugriff auf Besitzerebene auf das Notizbuch dar. „Contributor“ stellt Lese-/Schreibzugriff auf das Notizbuch dar. „Reader“ stellt schreibgeschützten Zugriff auf das Notizbuch dar. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|sectionGroups|[SectionGroup](sectiongroup.md)-Sammlung|Die Abschnittsgruppen im Notizbuch. Schreibgeschützt. Lässt Nullwerte zu.|
|Abschnitte|[OnenoteSection](section.md) -Auflistung|Die Abschnitte im Notizbuch. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Notizbuch abrufen](../api/notebook-get.md) | [Notebook](notebook.md) |Dient zum Lesen der Eigenschaften und Beziehungen des Notizbuchs.|
|[getRecentNotebooks](../api/notebook-getrecentnotebooks.md) | [recentNotebook](recentnotebook.md)-Sammlung | Dient zum Abrufen einer Sammlung der zuletzt geöffneten Notizbücher des Benutzers. |
|[getNotebookFromWebUrl](../api/notebook-getnotebookfromweburl.md) | [Notebook](notebook.md) | Abrufen der Eigenschaften und die Beziehungen eines Notebook-Objekts verwenden den URL-Pfad. |
|[Abschnittsgruppe erstellen](../api/notebook-post-sectiongroups.md) |[SectionGroup](sectiongroup.md)| Dient zum Erstellen einer Abschnittsgruppe durch Veröffentlichung in der SectionGroups-Sammlung im angegebenen Notizbuch.|
|[Abschnittsgruppen auflisten](../api/notebook-list-sectiongroups.md) |[SectionGroup](sectiongroup.md)-Sammlung| Dient zum Abrufen einer Sammlung von Abschnittsgruppen im angegebenen Notizbuch.|
|[Abschnitt erstellen](../api/notebook-post-sections.md) |[OnenoteSection](section.md)| Dient zum Erstellen eines Abschnitts durch Veröffentlichung in der Sections-Sammlung im angegebenen Notizbuch.|
|[Abschnitte auflisten](../api/notebook-list-sections.md) |[OnenoteSection](section.md) -Auflistung| Dient zum Abrufen einer Sammlung von Abschnitten im angegebenen Notizbuch.|
|[copyNotebook](../api/notebook-copynotebook.md)| Keine | Kopiert ein Notizbuch.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
