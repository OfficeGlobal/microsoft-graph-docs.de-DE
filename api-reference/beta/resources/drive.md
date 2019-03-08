---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Laufwerk
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 82a14f6462604b732119b90d037b2fab711df5af
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480992"
---
# <a name="drive-resource-type"></a>Drive-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die drive-Ressource ist das Objekt der obersten Ebene innerhalb des OneDrive eines Benutzers oder einer Dokumentbibliothek in SharePoint.

OneDrive-Benutzern steht immer mindestens ein Laufwerk zur Verfügung, das Standardlaufwerk. Benutzern ohne OneDrive-Lizenz steht möglicherweise kein Standardlaufwerk zur Verfügung.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer Laufwerksressource.

Die **drive**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "activities",
    "createdBy",
    "createdDateTime",
    "description",
    "lastModifiedBy",
    "lastModifiedDateTime",
    "name",
    "webUrl",
    "items",
    "root",
    "special",
    "system"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "following": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "items": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "quota": { "@odata.type": "microsoft.graph.quota" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "special": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "system": { "@odata.type": "microsoft.graph.systemFacet" },
  "webUrl": "url"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft             | Typ                          | Beschreibung                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| createdBy            | [identitySet][]               | Die Identität des Benutzers, des Geräts oder der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.                                                                                                                                                  |
| createdDateTime      | dateTimeOffset                | Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.                                                                                                                                                                                       |
| description          | Zeichenfolge                        | Stellt eine für den Benutzer sichtbare Beschreibung des Laufwerks bereit. Lese-/Schreibzugriff.
| driveType            | String                        | Beschreibt den Typ des Laufwerks, der durch diese Ressource dargestellt wird. Persönliche OneDrive-Laufwerke geben `personal` zurück. OneDrive for Business gibt `business` zurück. SharePoint-Dokumentbibliotheken geben `documentLibrary` zurück. Schreibgeschützt. |
| id                   | String                        | Der eindeutige Bezeichner des Laufwerks. Schreibgeschützt.                                                                                                                                                                                   |
| lastModifiedBy       | [identitySet][]               | Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.                                                                                                                                           |
| lastModifiedDateTime | dateTimeOffset                | Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.                                                                                                                                                                             |
| name                 | string                        | Der Name des Elements. Lese-/Schreibzugriff.                                                                                                                                                                                                |
| owner                | [identitySet](identityset.md) | Optional.  Das Benutzerkonto, das das Laufwerk besitzt. Schreibgeschützt.                                                                                                                                                                       |
| quota                | [quota](quota.md)             | Optional.  Informationen zum Speicherkontingent des Laufwerks. Schreibgeschützt.                                                                                                                                                          |
| sharepointIds        | [sharepointIds][]             | Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.                                                                                                                                                         |
| System               | [systemFacet][]               | Falls vorhanden, gibt an, dass es sich um ein vom System verwaltetes Laufwerk handelt. Schreibgeschützt.
| webUrl               | String (URL)                  | URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ                                 | Beschreibung
|:-------------|:-------------------------------------|:-----------------------
| Aktivitäten   | [itemActivity][]-Sammlung          | Die Liste der letzten Aktivitäten, die für dieses Laufwerk durchgeführt wurden.
| Elemente        | [driveitem](driveitem.md) collection | Alle im Laufwerk enthaltenen Elemente. Schreibgeschützt. Lässt Nullwerte zu.
| root         | [driveitem](driveitem.md)            | Der Stammordner des Laufwerks. Schreibgeschützt.
| Sonderfall      | [driveitem](driveitem.md) collection | Sammlung gemeinsamer Ordner, die  in OneDrive zur Verfügung stehen. Schreibgeschützt. Lässt Nullwerte zu.
| following    | [Driveitem](driveitem.md)-Sammlung | Die Liste von Elementen, denen der Benutzer folgt. Nur in OneDrive for Business.

## <a name="methods"></a>Methoden

|                        Häufige Aufgaben                         |         HTTP-Methode         |
| :--------------------------------------------------------- | :-------------------------- |
| [Abrufen der Laufwerks-Metadaten eines anderen Laufwerks][drive-get]           | `GET /drives/{drive-id}`    |
| [Abrufen des Stammordners des Standardlaufwerks des Benutzers][item-get]       | `GET /drive/root`           |
| [Auflisten der Aktivitäten unter dem Laufwerk][drive-activities]        | `GET /drive/activities`     |
| [Auflisten der Elemente, denen gefolgt wird][drive-following]                     | `GET /drive/following`      |
| [Auflisten der untergeordneten Elemente des Laufwerks][item-children]             | `GET /drive/root/children`  |
| [Auflisten der Änderungen für alle Elemente auf dem Laufwerk][item-changes]    | `GET /drive/root/delta`     |
| [Suchen nach Elementen auf dem Laufwerk][item-search]               | `GET /drive/root/search`    |
| [Abrufen spezieller Ordner](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

In der vorstehenden Tabelle verwenden die Beispiele `/drive`, andere Pfade sind jedoch ebenfalls gültig.

[itemActivity]: itemactivity.md
[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-activities]: ../api/activities-list.md
[drive-following]: ../api/drive-list-following.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": {
    "Resources/Drive": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/drive.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
