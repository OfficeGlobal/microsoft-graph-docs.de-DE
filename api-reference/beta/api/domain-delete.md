---
title: Domäne löschen
description: Dient zum Löschen einer Domäne aus einem Mandanten.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b17d8fea23b48cae8ed3227952fb952297a9aaa0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513207"
---
# <a name="delete-domain"></a>Domäne löschen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Dient zum Löschen einer Domäne aus einem Mandanten.

> **Wichtig:** Gelöschte Domänen können nicht wiederhergestellt werden.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).


|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Domain.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.

## <a name="request-headers"></a>Anforderungsheader

| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |
| Content-Type  | application/json |

## <a name="request-body"></a>Anforderungstext

Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Es wird keine Antworttext zurückgegeben.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```

##### <a name="response"></a>Antwort

Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
