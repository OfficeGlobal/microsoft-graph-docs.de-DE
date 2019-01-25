---
title: Löschen einer historyItem
description: Löschen Sie ein vorhandenes Verlaufselement für einen vorhandenen Benutzer-Aktivität hinzu.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: b3e9a505c47c4d43aff71d5b4e40f08e3fe29d2b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520424"
---
# <a name="delete-a-historyitem"></a>Löschen einer historyItem

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Löschen Sie ein vorhandenes Verlaufselement für einen vorhandenen Benutzer-Aktivität hinzu.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).


|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | UserActivity.ReadWrite.CreatedByApp    |
|Delegiert (persönliches Microsoft-Konto) | UserActivity.ReadWrite.CreatedByApp    |
|Anwendung | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a>Anforderungsheader

|Name | Typ | Beschreibung|
|:----|:-----|:-----------|
|Authorization | string | Bearer {token}. Erforderlich.|

## <a name="request-body"></a>Anforderungstext

Keine Anforderungstext.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode die `204 No Content` Antwortcode, wenn das Historienelement gelöscht wurde.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```

##### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-delete-historyitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
