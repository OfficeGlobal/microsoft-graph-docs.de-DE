---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Laufwerk
ms.openlocfilehash: 0b178967f7eb8da8bdf8584bb13a7d4f9950392b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="drive-resource-type"></a>Drive-Ressourcentyp

Die drive-Ressource ist das Objekt der obersten Ebene innerhalb des OneDrive eines Benutzers oder einer Dokumentbibliothek in SharePoint.

OneDrive-Benutzern steht immer mindestens ein Laufwerk zur Verfügung, das Standardlaufwerk. Benutzern ohne OneDrive-Lizenz steht möglicherweise kein Standardlaufwerk zur Verfügung.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer Laufwerksressource.

Die **drive**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.drive",
       "keyProperty": "id", 
       "optionalProperties": [ "activities", "createdBy", "createdDateTime", "description", "lastModifiedBy", "lastModifiedDateTime", "name", "webUrl", "items", "root", "special", "system"] } -->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
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
| items        | [driveitem](driveitem.md) collection | Alle im Laufwerk enthaltenen Elemente. Schreibgeschützt. Lässt Nullwerte zu.
| root         | [driveitem](driveitem.md)            | Der Stammordner des Laufwerks. Schreibgeschützt.
| Sonderfall      | [driveitem](driveitem.md) collection | Sammlung gemeinsamer Ordner, die  in OneDrive zur Verfügung stehen. Schreibgeschützt. Lässt Nullwerte zu.

## <a name="methods"></a>Methoden

|                        Häufige Aufgaben                         |         HTTP-Methode         |
| :--------------------------------------------------------- | :-------------------------- |
| [Abrufen der Laufwerks-Metadaten eines anderen Laufwerks][drive-get]           | `GET /drives/{drive-id}`    |
| [Abrufen des Stammordners des Standardlaufwerks des Benutzers][item-get]       | `GET /drive/root`           |
| [Auflisten der untergeordneten Elemente des Laufwerks][item-children]             | `GET /drive/root/children`  |
| [Auflisten der Änderungen für alle Elemente auf dem Laufwerk][item-changes]    | `GET /drive/root/delta`     |
| [Suchen nach Elementen auf dem Laufwerk][item-search]               | `GET /drive/root/search`    |
| [Abrufen spezieller Ordner](../api/drive_get_specialfolder.md) | `GET /drive/special/{name}` |

In der vorstehenden Tabelle verwenden die Beispiele `/drive`, andere Pfade sind jedoch ebenfalls gültig.

[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-get]: ../api/drive_get.md
[item-get]: ../api/driveitem_get.md
[item-changes]: ../api/driveitem_delta.md
[item-search]: ../api/driveitem_search.md
[item-children]: ../api/driveitem_list_children.md


<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->
