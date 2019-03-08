---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 435544db272b26e6fe3ac0e09803858eec9d05f6
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480880"
---
# <a name="listitem-resource"></a>ListItem-Ressource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Diese Ressource stellt ein Element in einer SharePoint-**[Liste][]** dar.
Spaltenwerte in der Liste sind über das `fieldValueSet`-Wörterbuch verfügbar.

## <a name="tasks-on-a-listitem"></a>Aufgaben zu einem listItem

Die folgenden Aufgaben sind für **listItem**-Ressourcen verfügbar.
Alle Beispiele unten beziehen sich auf eine **[Liste][]**, z. B.: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.

| Häufige Aufgaben                    | HTTP-Methode
|:-------------------------------|:------------------------
| [Get][]                        | GET /items/{item-id}
| [Abrufen von Spaltenwerten][Get]       | GET /items/{item-id}?expand=fields
| [Analysen abrufen][]              | /Items/{Item-ID}/Analytics abrufen
| [Aktivitäten nach Intervall abrufen][] | /Items/{item-id}/getActivitiesByInterval abrufen
| [Create][]                     | POST /items
| [Delete][]                     | DELETE /items/{item-id}
| [Update][]                     | PATCH /items/{item-id}
| [Aktualisieren von Spaltenwerten][Update] | PATCH /items/{item-id}/fields

[Get]: ../api/listitem-get.md
[Analysen abrufen]: ../api/itemanalytics-get.md
[Aktivitäten nach Intervall abrufen]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **listItem**-Ressource.

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.listItem"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "versions": [{"@odata.type": "microsoft.graph.listItemVersion"}],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "url"
}
```

## <a name="properties"></a>Eigenschaften

Die **listItem**-Ressource weist folgende Eigenschaften auf.

| Eigenschaftenname | Typ                | Beschreibung
|:--------------|:--------------------|:-------------------------------
| contentType   | [contentTypeInfo][] | Der Inhaltstyp dieses Listenelements

Die folgenden Eigenschaften werden von ** [baseItem][]** geerbt.

| Eigenschaftenname        | Typ              | Beschreibung
|:---------------------|:------------------|:----------------------------------
| id                   | Zeichenfolge            | Der eindeutige Bezeichner des Elements. Schreibgeschützt.
| name                 | Zeichenfolge            | Der Name/Titel des Elements.
| createdBy            | [identitySet][]   | Die Identität des Erstellers dieses Elements. Schreibgeschützt.
| createdDateTime      | DateTimeOffset    | Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.
| description          | string            | Der beschreibende Text für das Element.
| eTag                 | string            | ETag für das Element. Schreibgeschützt.                                                          |
| lastModifiedBy       | [identitySet][]   | Die Identität derPerson, die dieses Element zuletzt geändert hat. Schreibgeschützt.
| lastModifiedDateTime | DateTimeOffset    | Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.
| parentReference      | [itemReference][] | Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.
| sharepointIds        | [sharepointIds][] | Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.
| webUrl               | String (URL)      | URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.

## <a name="relationships"></a>Beziehungen

 Die **listItem**-Ressource weist folgende Beziehungen zu anderen Ressourcen auf.

| Beziehungsname | Typ                           | Beschreibung
|:------------------|:-------------------------------|:-------------------------------
| Aktivitäten        | [ItemActivity][]-Sammlung    | Die Liste der letzten Aktivitäten, die für dieses Element durchgeführt wurden.
| Analyse         | [itemAnalytics][]-Ressource     | Analysen zu den Ansichts Aktivitäten, die für dieses Element durchgeführt wurden.
| driveItem         | [driveItem][]                  | Für Dokumentbibliotheken macht die **DriveItem** Beziehung das ListItem als ** [DriveItem][]** verfügbar
| fields            | [fieldValueSet][]              | Die Werte der für dieses Listenelement festgelegten Spalte.
| versions          | [listItemVersion][] -Sammlung | Die Liste der vorherigen Versionen des Listenelements.

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/listitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
