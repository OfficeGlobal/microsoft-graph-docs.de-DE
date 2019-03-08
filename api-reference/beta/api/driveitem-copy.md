---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Kopieren einer Datei oder eines Ordners
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: cdb22395cfde6820eb5450f39bd1e3408a4f82b2
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481902"
---
# <a name="copy-a-driveitem"></a>DriveItem kopieren

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Erstellt asynchron eine Kopie eines [driveItem][item-resource] (einschließlich aller untergeordneten Elemente) unter einem neuen übergeordneten Element oder mit einem neuen Namen.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Files.ReadWrite, Files.ReadWrite.All    |
|Anwendung | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

### <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.


| Name            | Wert                                          | Beschreibung                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| parentReference | [ItemReference](../resources/itemreference.md) | Optional.  Verweis auf das übergeordnete Element, in dem die Kopie erstellt wird.                                         |
| name            | string                                         | Optional.  Der neue Name der Kopie. Wenn dieser nicht angegeben wird, wird der gleiche Namen wie für das Original verwendet.    |

**Hinweis:** Die _ParentReference_ sollte die Parameter `driveId` und `id` für den Zielordner enthalten.

## <a name="example"></a>Beispiel

In diesem Beispiel wird eine von `{item-id}` mit einem `driveId`- und `id`-Wert identifizierte Datei in einen Ordner kopiert.
Die neue Kopie der Datei erhält den Namen `contoso plan (copy).txt`.

<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "driveId": "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B",
    "id": "DCD0D3AD-8989-4F23-A5A2-2C086050513F"
  },
  "name": "contoso plan (copy).txt"
}
```

## <a name="response"></a>Antwort

Die Methode gibt zusammen mit der Annahme der Anforderung Details zur [Überwachung des Fortschritts](/graph/long-running-actions-overview) des Kopiervorgangs zurück.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

Der Wert des `Location`-Headers enthält eine Dienst-URL, die den aktuellen Status des Kopiervorgangs zurückgibt. Anhand dieser Informationen können Sie [herausfinden, wann der Kopiervorgang abgeschlossen ist](/graph/long-running-actions-overview).

### <a name="remarks"></a>Hinweise

In vielen Fällen wird die Aktion zum Kopieren asynchron durchgeführt. Die Antwort der API gibt nur an, dass der Kopiervorgang akzeptiert oder abgelehnt wurde, wenn der Zieldateiname zum Beispiel bereits verwendet wird.

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-copy.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
