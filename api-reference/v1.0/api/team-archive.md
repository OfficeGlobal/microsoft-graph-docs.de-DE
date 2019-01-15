---
title: Archiv-team
description: 'Archivieren Sie das angegebene Team. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: c7ac186eeb937b1dda0b1df4878260e61fe30b18
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016639"
---
# <a name="archive-team"></a>Archiv-team



Archivieren Sie das angegebene [Team](../resources/team.md). Wenn ein Team archiviert wird, können Benutzer nicht mehr senden wie Nachrichten auf einem beliebigen Kanal im Team, bearbeiten das Team Name, Beschreibung oder andere Einstellungen oder im Allgemeinen die meisten Änderungen an das Team vornehmen.
Mitgliedschaftsänderungen an das Team weiterhin zugelassen werden.

Archivierung ist ein asynchroner Vorgang. Nach Abschluss des Vorgangs Async erfolgreich, die nach einer Antwort vom diese API auftreten können, ist ein Team archiviert.

Zum Archivieren von Team benötigen die Teams und der [Gruppe](../resources/group.md) Besitzer.

Um ein Team aus den archivierten Zustand wiederherzustellen, verwenden Sie die API zu [Öffnen](team-unarchive.md).

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
POST /teams/{id}/archive
```
## <a name="request-headers"></a>Anforderungsheader
| Header       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich.  |

## <a name="request-body"></a>Anforderungstext
In der Anforderung kann _optional_ umfassen die `shouldSetSpoSiteReadOnlyForMembers` Parameter in einem JSON body, wie folgt.
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
Dieser optionale Parameter definiert, ob Festlegen von Berechtigungen für Teammitglieder den Schreibschutz für die Sharepoint Online-Website mit dem Team verknüpft ist. Festlegen der Steuerelementvorlage auf False oder im Textkörper auslassen führt vollständig in diesem Schritt wird übersprungen.

## <a name="response"></a>Antwort

Wenn die Archivierung erfolgreich gestartet wurde, gibt diese Methode einen `202 Accepted` Antwortcode. Die Antwort enthält außerdem eine `Location` Kopf, der den Speicherort der die [TeamsAsyncOperation](../resources/teamsasyncoperation.md) enthält, die zum Behandeln des Teams Archivierung erstellt wurde. Überprüfen Sie den Status des Vorgangs Archivierung, indem er eine GET-Anforderung an diesen Speicherort.

## <a name="example"></a>Beispiel
#### <a name="request"></a>Anforderung
Es folgt ein Beispiel für eine Anforderung.
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/archive
```
#### <a name="response"></a>Antwort
Es folgt ein Beispiel für eine Antwort.
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
