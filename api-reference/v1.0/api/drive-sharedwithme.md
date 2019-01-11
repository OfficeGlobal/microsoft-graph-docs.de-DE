---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Mit mir geteilte Dateien auflisten
localization_priority: Priority
ms.openlocfilehash: 89ad3a5fc8aa12dd6865a629fd80b5a72623302c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889425"
---
# <a name="list-items-shared-with-the-signed-in-user"></a>Elemente auflisten, die für den angemeldeten Benutzer freigegeben sind

Mit dieser API können Sie eine Sammlung von Ressourcen des Typs [DriveItem](../resources/driveitem.md) abrufen, die für den Besitzer der Ressource des Typs [Drive](../resources/drive.md) freigegeben wurden.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Files.Read.All, Files.ReadWrite.All    |
|Anwendung | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

**Hinweis:** Die /sharedWithMe-Anforderung funktioniert zwar mit Files.Read- oder Files.ReadWrite-Berechtigungen, es kann jedoch sein, dass einige Eigenschaften fehlen.
Zusätzlich gilt: Ohne eine der Berechtigungen des Typs **All** ist kein Zugriff auf die von dieser API zurückgegebenen freigegebenen Elemente möglich.

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "request", "name": "shared-with-me", "scopes": "files.read", "tags": "service.graph", "target": "action" } -->

```http
GET /me/drive/sharedWithMe
```

## <a name="response"></a>Antwort

Dadurch wird eine Sammlung von [DriveItem](../resources/driveitem.md)-Ressourcen, zurückgegeben, die die DriveItem-Ressourcen enthalten, die für den Besitzer des Laufwerks freigegeben wurden. Da es sich bei dem Laufwerk um das Standardlaufwerk des Benutzers handelt, werden in diesem Beispiel Elemente zurückgegeben, die für den angemeldeten Benutzer freigegeben sind.

<!-- {"blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc",
      "remoteItem": {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    },
    {
      "id": "1312def",
      "remoteItem": {
        "id": "1991210caf!1991",
        "name": "Team Roster.xlsx",
        "file": { },
        "size": 37619,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a>Bemerkungen

DriveItems, die von der **SharedWithMe**-Aktion zurückgegeben werden, enthalten immer das [**remoteItem**](../resources/remoteitem.md)-Facet, das angibt, dass es sich um Elemente von einem anderen Laufwerk handelt. Um auf die freigegebenen DriveItem Ressourcen zuzugreifen, müssen Sie eine Anforderung anhand der Angaben in **remoteItem** im folgenden Format stellen:

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!-- {
  "type": "#page.annotation",
  "description": "List the items shared with the owner of a drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Sharing/Shared with me"
} -->
