---
title: DriveItemVersion-Ressource erhalten (Vorschau)
description: Rufen Sie die Metadaten für eine bestimmte Version eines DriveItem ab.
localization_priority: Normal
ms.openlocfilehash: f0c5611b769ed5e8adb63550a76016a055245504
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853711"
---
# <a name="get-a-driveitemversion-resource-preview"></a>DriveItemVersion-Ressource erhalten (Vorschau)

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Rufen Sie die Metadaten für eine bestimmte Version eines [DriveItem](../resources/driveitem.md) ab.

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
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [DriveItemVersion](../resources/driveitemversion.md)-Objekt im Antworttext zurückgegeben.


## <a name="example"></a>Beispiel

In diesem Beispiel wird die Version einer Datei auf dem Laufwerk des aktuellen Benutzers abgerufen.

### <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a>Antwort

Dadurch wird eine Sammlung von Versionen zurückgegeben:

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "D4990684-58CE-4FAB-9B87-D6C49E74F298",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "size": 123
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
