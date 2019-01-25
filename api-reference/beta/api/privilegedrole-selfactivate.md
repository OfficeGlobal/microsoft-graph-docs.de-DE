---
title: 'PrivilegedRole: SelfActivate'
description: Aktivieren Sie die Rolle, die an die anfordernde Person zugewiesen ist.
localization_priority: Normal
ms.openlocfilehash: e0197599373246853906b879c0f3d13e61a45244
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515069"
---
# <a name="privilegedrole-selfactivate"></a>PrivilegedRole: SelfActivate

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aktivieren Sie die Rolle, die an die anfordernde Person zugewiesen ist.

>**Hinweis:** Eine effektive Dezember 2018, diese API wird nicht mehr unterstützt und sollte nicht verwendet werden. Verwenden Sie stattdessen die [PrivilegedRoleAssignmentRequest erstellen](privilegedroleassignmentrequest-post.md) .


## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

Der Requestor kann nur aufgerufen ```selfActivate``` für die Rolle, die ihm zugewiesen ist.
 

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

Beachten Sie, dass ``<id>`` ist die Ziel-Rolle-ID.
## <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

| Parameter    | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Grund|string|Optional. Beschreibung der Grund für diese Rolle Aktivierung.|
|duration|string|Optional. Gültige Werte werden konnte ```min``` (minimale Aktivierung Dauer), ```default``` (Standard-Aktivierung Dauer für die Rolle), oder einen double-Wert an, wie viele Stunden die Aktivierung ist. Die angegebene Dauer darf nicht länger als die Rolle Aktivierung Dauer aus der Einstellung der Rolle sein. |
|ticketNumber|string|Optional. Die Ticket-Nummer, die zum Nachverfolgen von dieser Rolle-Aktivierung verwendet wird.|
|ticketSystem|string|Optional. Das System Ticket.|

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) -Objekts in der Antworttext.

Beachten Sie, dass der Mandant muss auf den PIM registriert werden. Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.
## <a name="example"></a>Beispiel
Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfActivate
Content-type: application/json
Content-length: 142

{
  "reason": "reason-value",
  "duration": "duration-value",
  "ticketNumber": "ticketNumber-value",
  "ticketSystem": "ticketSystem-value"
}
```

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. 

>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole: selfActivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-selfactivate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
