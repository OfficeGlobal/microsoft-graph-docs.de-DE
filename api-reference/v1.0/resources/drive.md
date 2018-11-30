---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Laufwerk
ms.openlocfilehash: f4deeb949a65c11e51137c850ccde67b50a38827
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016508"
---
# <a name="drive-resource-type"></a>Drive-Ressourcentyp

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
    "sharepointIds",
    "special",
    "system"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.drive"
}-->

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
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
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
| System-               | [systemFacet][]               | Falls vorhanden, gibt an, dass es sich um ein vom System verwaltetes Laufwerk handelt. Schreibgeschützt.
| webUrl               | String (URL)                  | URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ                                 | Beschreibung
|:-------------|:-------------------------------------|:-----------------------
| Elemente        | [DriveItem](driveitem.md) -Auflistung | Alle im Laufwerk enthaltenen Elemente. Schreibgeschützt. Lässt Nullwerte zu.
| root         | [DriveItem](driveitem.md)            | Der Stammordner des Laufwerks. Schreibgeschützt.
| Sonderfall      | [DriveItem](driveitem.md) -Auflistung | Sammlung gemeinsamer Ordner, die  in OneDrive zur Verfügung stehen. Schreibgeschützt. Lässt Nullwerte zu.
| Liste         | [List](list.md)                      | Für Laufwerke in SharePoint-Liste der zugrunde liegenden Dokumentbibliothek. Schreibgeschützt. Lässt Nullwerte zu.

## <a name="methods"></a>Methoden

|                        Häufige Aufgaben                         |         HTTP-Methode         |
| :--------------------------------------------------------- | :-------------------------- |
| [Abrufen der Laufwerks-Metadaten eines anderen Laufwerks][drive-get]           | `GET /drives/{drive-id}`    |
| [Abrufen des Stammordners des Standardlaufwerks des Benutzers][item-get]       | `GET /drive/root`           |
| [Auflisten der untergeordneten Elemente des Laufwerks][item-children]             | `GET /drive/root/children`  |
| [Auflisten der Änderungen für alle Elemente auf dem Laufwerk][item-changes]    | `GET /drive/root/delta`     |
| [Suchen nach Elementen auf dem Laufwerk][item-search]               | `GET /drive/root/search`    |
| [Abrufen spezieller Ordner](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

In der vorstehenden Tabelle verwenden die Beispiele `/drive`, andere Pfade sind jedoch ebenfalls gültig.

[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md


<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/drive.md:
      Found potential enums in resource example that weren't defined in a table:(personal,business,documentLibrary) are in resource, but () are in table"
  ],
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->
