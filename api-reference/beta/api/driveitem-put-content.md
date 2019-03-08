---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Hochladen kleiner Dateien
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 151d7c9479068c5fdcecfb5a04166900bd527230
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482273"
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a>Inhalte eines DriveItem hochladen oder ersetzen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Mit der einfachen Upload-API können Sie den Inhalt einer neuen Datei bereitstellen oder den Inhalt einer vorhandenen Datei in einem einzigen API-Aufruf aktualisieren . Diese Methode unterstützt nur Dateien, die bis zu 4MB groß sind.

Informationen zum Hochladen großer Dateien finden Sie unter [Große Dateien mit einer Uploadsitzung hochladen](driveitem-createuploadsession.md).

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Files.ReadWrite, Files.ReadWrite.All    |
|Anwendung | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request-to-replace-an-existing-item"></a>HTTP-Anforderung (um ein vorhandenes Element zu ersetzen)

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a>HTTP-Anforderung (um eine neue Datei hochzuladen)

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a>Anforderungstext

Der Inhalt des Anforderungstexts sollte den binären Stream der hochzuladenden Datei sein.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird ein [driveItem](../resources/driveitem.md)-Objekt im Antworttext der neu erstellten oder aktualisierten Datei zurückgegeben.

## <a name="example-upload-a-new-file"></a>Beispiel (Hochladen einer neuen Datei)

In diesem Beispiel wird die Zeichenfolge "Die Inhalte der Datei hier einfügen" auf dem angemeldeten Benutzerlaufwerk in einer Datei mit dem Namen FileB.txt in den Ordner FolderA hochgeladen.

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird eine [driveItem][item-resource]-Ressource im Antworttext der neu erstellten Datei zurückgegeben.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "FileB.txt",
  "size": 35,
  "file": { }
}
```

## <a name="example-updating-an-existing-file"></a>Beispiel (Aktualisieren einer vorhandenen Datei)

In diesem Beispiel wird der Inhalt einer Datei durch eine bekannte ID ersetzt.

<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird eine [driveItem][item-resource]-Ressource im Antworttext der neu erstellten Datei zurückgegeben.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "FileB.txt",
  "size": 35,
  "file": { }
}
```

## <a name="error-responses"></a>Fehlerantworten

Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-put-content.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
