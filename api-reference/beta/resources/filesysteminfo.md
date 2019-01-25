---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: fileSystemInfo
localization_priority: Normal
ms.openlocfilehash: e2dfac79f5c7d511cab11c076d697940a01f4c7c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524695"
---
# <a name="filesysteminfo-facet"></a>FileSystemInfo-Facet

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die Ressource FileSystemInfo enthält Eigenschaften, die vom lokalen Dateisystem des Geräts für die lokale Version eines Elements gemeldet werden. Diese Facet kann zum Angeben des letzten Änderungsdatums oder des Erstellungsdatums des Elements verwendet werden, wie es auf dem lokalen Gerät gespeichert war.

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
| **lastAccessedDateTime** | DateTimeOffset | Das UTC-Datum und die UTC-Uhrzeit des letzten Zugriffs auf die Datei. Nur für die Liste der zuletzt verwendeten Dateien verfügbar. |
| **lastModifiedDateTime** | DateTimeOffset | Das UTC-Datum und die UTC-Uhrzeit der letzten Änderung der Datei auf einem Client.                                                        |

## <a name="notes"></a>Anmerkungen

Werte für createdDateTime und lastModifiedDateTime unterscheiden sich von den gleichen Eigenschaften auf der Ressource DriveItem. Die Werte für die Ressource DriveItem sind Erstellungsdatum und -uhrzeit, wie sie vom Dienst erfasst werden. Die in der Ressource FileSystemInfo gespeicherten Werte werden vom Client bereitgestellt.

Beispiel: Wenn eine Datei am Montag auf dem Gerät erstellt wurde, aber erst am Dienstag in den Dienst hochgeladen wurde, muss der Client, der die Datei hochlädt, die Facet `fileSystemInfo` schreiben, um das Erstellungsdatum am Montag einzubeziehen. Wenn die Metadaten des Elements abgerufen werden, wird als Erstellungsdatum für das Element Dienstag angegeben. Die Facet `fileSystemInfo` zeigt jedoch das ursprüngliche Erstellungsdatum am Montag an.

Diese Eigenschaften sind lese- und schreibgeschützt. Wenn Sie eine Datei hochladen und die lokalen Client-Werte für diese Felder kennen, sollten Sie diese bei der Anfrage einbeziehen.

Wenn der Inhalt der Datei aktualisiert wird und diese Eigenschaften nicht angegeben werden, wird **lastModifiedDateTime** automatisch auf die aktuelle Uhrzeit zurückgesetzt.

## <a name="remarks"></a>Hinweise

* **lastAccessedDateTime** ist für Elemente in SharePoint Online oder OneDrive for Business nicht verfügbar.

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "The fileSystemInfo facet provides information about date created and modified by clients.",
  "keywords": "fileSystemInfo,client,system info,onedrive",
  "section": "documentation",
  "tocPath": "Facets/FileSystemInfo",
  "suppressions": [
    "Error: /api-reference/beta/resources/filesysteminfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
