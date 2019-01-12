---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Zuletzt verwendete Dateien auflisten
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3548a708084da5b5c22bd31be1130630a577d7bb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922725"
---
# <a name="list-recent-files"></a>Zuletzt verwendete Dateien auflisten

Dient zum Auflisten eines Satzes von Elementen, die zuletzt von dem angemeldeten Benutzer verwendet wurden. Diese Sammlung enthält Elemente, die sich in dem Laufwerk des Benutzers befinden sowie Elemente in anderen Laufwerken, auf die dieser Zugriff hat.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Anwendung | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "request",
       "name": "view-recent-files", 
       "scopes": "files.read",
       "tags": "service.graph",
       "target": "action" } -->

```http
GET /me/drive/recent
```

## <a name="response"></a>Antwort

Mit dieser Methode wird eine Sammlung von [DriveItem](../resources/driveitem.md)-Ressourcen für Elemente zurückgegeben, auf die der Besitzer des Laufwerks vor kurzem zugegriffen hat.

<!-- { "blockType": "response",
       "@odata.type": "Collection(microsoft.graph.driveItem)",
       "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "remoteItem":
      {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      },
      "fileSystemInfo": {
        "lastAccessedDateTime": "2017-02-20T19:13:00Z"
      }
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "file": { },
      "size": 37810,
      "parentReference": {
        "driveId": "1312def",
        "id": "1312def!123"
      },
      "fileSystemInfo": {
        "lastAccessedDateTime": "2017-02-20T16:43:21Z"
      }
    }
  ]
}
```

## <a name="remarks"></a>Hinweise

Einige driveItems, die von der **recent**-Aktion zurückgegeben werden, enthalten immer das **remoteItem**-Facet, das angibt, dass es sich um Elemente von einem anderen Laufwerk handelt. Um auf das ursprüngliche DriveItem-Objekt zuzugreifen, müssen Sie eine Anforderung anhand der Angaben in **remoteItem** im folgenden Format stellen:

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of recently used files for the owner of the drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Drives/Recent files"
} -->
