---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Wiederherstellen einer früheren Version eines SharePoint-Listenelements
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 20cf0460aa679fc40a4bb11d0887bc4946ddcd74
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482084"
---
# <a name="restore-a-previous-version-of-a-listitem"></a>Frühere Version eines SharePoint-Listenelements wiederherstellen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellen Sie eine frühere Version eines Listenelements als aktuelle Version wieder her. Dadurch wird eine neue Version mit dem Inhalt der vorherigen Version erstellt, aber alle vorhandenen Versionen des Elements bleiben erhalten.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|            Berechtigungstyp             |         Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)          |
| :------------------------------------- | :----------------------------------------------------------- |
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All |
| Delegiert (persönliches Microsoft-Konto) | N/V                                                          |
| Anwendung                            | Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a>Anforderungstext

Es ist kein Anforderungstexts erforderlich.

## <a name="example"></a>Beispiel

In diesem Beispiel wird eine Version eines von `{item-id}` und `{version-id}` identifizierten Listenelements wiederhergestellt.

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a>Antwort

Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No content` zurück.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/listitemversion-restore.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
