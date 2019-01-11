---
title: Auflisten von Versionen einer DriveItem
description: OneDrive und SharePoint können auch so konfiguriert werden, dass für Dateien ein Verlauf beibehalten wird.
localization_priority: Normal
ms.openlocfilehash: 6093371e6ef461b82fd2b5c92b22da7333f7e342
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855489"
---
# <a name="listing-versions-of-a-driveitem"></a>Auflisten von Versionen einer DriveItem

OneDrive und SharePoint können auch so konfiguriert werden, dass für Dateien ein Verlauf beibehalten wird.
Je nach Dienst und Konfiguration kann für jede Änderung beim Speichern der Datei eine neue Version erstellt werden, manuell oder nie.

Vorherige Versionen eines Dokuments können je nach Administratoreinstellungen für einen begrenzten Zeitraum beibehalten werden, diese können pro Benutzer oder Speicherort eindeutig sein.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Anwendung | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |


## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions
GET /groups/{group-id}/drive/{item-id}/versions
GET /me/drive/items/{item-id}/versions
GET /sites/{site-id}/drive/items/{item-id}/versions
GET /users/{user-id}/drive/items/{item-id}/versions
```

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [DriveItemVersion](../resources/driveitemversion.md)-Objekten im Antworttext zurückgegeben.


## <a name="example"></a>Beispiel

In diesem Beispiel werden die Versionen einer Datei auf dem Laufwerk des aktuellen Benutzers abgerufen.

### <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "request", "name": "get-previous-versions", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions
```

### <a name="response"></a>Antwort

Dadurch wird eine Sammlung von Versionen zurückgegeben:

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
      "size": 123
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z",
      "size": 62
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z",
      "size": 16
    }
  ]
}
```

## <a name="remarks"></a>Hinweise

OneDrive behält nicht die kompletten Metadaten für vorherige Versionen einer Datei bei.

Wenn Ihre App die Liste verfügbarer Versionen für eine Datei abruft, wird eine [DriveItemVersion](../resources/driveitemversion.md)-Ressource zurückgegeben, welche die verfügbaren Informationen zu der jeweiligen Version bereitstellt.


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
