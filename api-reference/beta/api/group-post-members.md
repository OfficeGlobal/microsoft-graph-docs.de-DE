---
title: Mitglied hinzufügen
description: Verwenden Sie diese API, um ein Mitglied einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die **member**-Navigationseigenschaft hinzuzufügen.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: ac21262858137074ed92978f0ab6530052fcc2de
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515678"
---
# <a name="add-member"></a>Mitglied hinzufügen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Verwenden Sie diese API, um ein Mitglied einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die **member**-Navigationseigenschaft hinzuzufügen.

Sie können Benutzer oder andere Gruppen hinzufügen. Wichtig: Sie können nur Benutzer zu Office 365-Gruppen hinzufügen.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Group.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung eines [directoryObject](../resources/directoryobject.md)- oder [user](../resources/user.md)- oder [group](../resources/group.md)-Objekts an, das hinzugefügt werden soll.

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a>Beispiel
#### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
Geben Sie im Textkörper Anforderung eine JSON-Darstellung der die `id` des Objekts [DirectoryObject](../resources/directoryobject.md), [Benutzer](../resources/user.md)oder [Gruppe](../resources/group.md) hinzufügen möchten.

#### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.
>**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
