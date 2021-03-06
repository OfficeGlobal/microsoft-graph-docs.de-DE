---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: FileSystemInfo
localization_priority: Normal
ms.openlocfilehash: 28f5cd631f9ea937150f9bb4c16e3775ea26d5d1
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482336"
---
# <a name="filesysteminfo-facet"></a>FileSystemInfo-Facet

Die Ressource **FileSystemInfo** enthält Eigenschaften, die vom lokalen Dateisystem des Geräts für die lokale Version eines Elements gemeldet werden. Diese Facet kann zum Angeben des letzten Änderungsdatums oder des Erstellungsdatums des Elements verwendet werden, wie es auf dem lokalen Gerät gespeichert war.

Das Facet ist verfügbar für die Eigenschaft „fileSystemInfo“ von Ressourcen des Typs [driveItem][item-resource].

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "lastAccessedDateTime"
  ],
  "@odata.type": "microsoft.graph.fileSystemInfo"
}-->

```json
{
  "createdDateTime" : "datetime",
  "lastAccessedDateTime": "datetime",
  "lastModifiedDateTime" : "datetime"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft                 | Typ           | Beschreibung                                                                                                          |
| :----------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------- |
| **createdDateTime**      | DateTimeOffset | Das UTC-Datum und die UTC-Uhrzeit der Erstellung der Datei auf einem Client.                                                              |
| **lastAccessedDateTime** | DateTimeOffset | Das UTC-Datum und die UTC-Uhrzeit des letzten Zugriffs auf die Datei. Nur für die [Liste der zuletzt verwendeten Dateien](../api/drive-recent.md) verfügbar. |
| **lastModifiedDateTime** | DateTimeOffset | Das UTC-Datum und die UTC-Uhrzeit der letzten Änderung der Datei auf einem Client.                                                        |

## <a name="notes"></a>Anmerkungen

Werte für **createdDateTime** und **lastModifiedDateTime** unterscheiden sich von den gleichen Eigenschaften auf der Ressource [DriveItem](driveitem.md). Die Werte für die Ressource DriveItem sind Erstellungsdatum und -uhrzeit, wie sie vom Dienst erfasst werden. Die in der Ressource **FileSystemInfo** gespeicherten Werte werden vom Client bereitgestellt.

Beispiel: Wenn eine Datei am Montag auf dem Gerät erstellt wurde, aber erst am Dienstag in den Dienst hochgeladen wurde, muss der Client, der die Datei hochlädt, die Facet `fileSystemInfo` schreiben, um das Erstellungsdatum am Montag einzubeziehen. Wenn die Metadaten des Elements abgerufen werden, wird als Erstellungsdatum für das Element Dienstag angegeben. Die Facet `fileSystemInfo` zeigt jedoch das ursprüngliche Erstellungsdatum am Montag an.

Diese Eigenschaften sind lese- und schreibgeschützt. Wenn Sie eine Datei hochladen und die lokalen Client-Werte für diese Felder kennen, sollten Sie diese bei der Anfrage einbeziehen.

Wenn der Inhalt der Datei aktualisiert wird und diese Eigenschaften nicht angegeben werden, wird **lastModifiedDateTime** automatisch auf die aktuelle Uhrzeit zurückgesetzt.

## <a name="remarks"></a>Hinweise

* **lastAccessedDateTime** ist für Elemente in SharePoint Online oder OneDrive for Business nicht verfügbar.

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The fileSystemInfo facet provides information about date created and modified by clients.",
  "keywords": "fileSystemInfo,client,system info,onedrive",
  "section": "documentation",
  "tocPath": "Facets/FileSystemInfo"
} -->
