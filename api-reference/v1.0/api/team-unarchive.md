---
title: Entpackt team
description: Wiederherstellen eines archivierten Teams. Dadurch wird die Möglichkeit zum Senden von Nachrichten und das Team Verhältnismäßigkeitsprinzips Mandanten und Team-Einstellungen Bearbeiten des Benutzers wiederhergestellt. Teams sind mithilfe des Archivs API archiviert.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 36e4183f53afab6ba836bacd909b616910dc0c42
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982078"
---
# <a name="unarchive-team"></a>Entpackt team



Wiederherstellen eines archivierten [Team](../resources/team.md). Dadurch wird die Möglichkeit zum Senden von Nachrichten und das Team Verhältnismäßigkeitsprinzips Mandanten und Team-Einstellungen Bearbeiten des Benutzers wiederhergestellt. Teams sind mit dem [Archiv](team-archive.md) API archiviert.

Unarchiving ist ein asynchroner Vorgang. Ein Team ist nicht archivierte, sobald der asynchrone Vorgang erfolgreich abgeschlossen wurde die nach einer Antwort vom diese API auftreten können.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Group.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Group.ReadWrite.All    |

> **Hinweis**: Diese API unterstützt Administratorberechtigungen. Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a>Anforderungsheader
| Header       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich.  |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn unarchiving erfolgreich gestartet wurde, gibt diese Methode einen `202 Accepted` Antwortcode. Die Antwort enthält außerdem eine `Location` Kopf, der den Speicherort der die [TeamsAsyncOperation](../resources/teamsasyncoperation.md) enthält, die zur Verarbeitung von unarchiving des Teams erstellt wurde. Überprüfen Sie den Status des Vorgangs unarchiving, indem er eine GET-Anforderung an diesen Speicherort.

## <a name="example"></a>Beispiel
#### <a name="request"></a>Anforderung
Es folgt ein Beispiel für eine Anforderung.
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a>Antwort
Es folgt ein Beispiel für eine Antwort.
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 9a9bb83f-6f35-4426-bb04-73ca43ad6cc8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Unarchive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
