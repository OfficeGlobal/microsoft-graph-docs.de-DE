---
title: Erstellen oder Ersetzen eines Zeitplans
description: Erstellen oder Ersetzen eines **Schedule** -Objekts.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ddae7a348d4150e8ef36974fecfe6b2c276b7f1d
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657483"
---
# <a name="create-or-replace-schedule"></a>Erstellen oder Ersetzen eines Zeitplans

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Erstellen oder Ersetzen eines [Schedule](../resources/schedule.md) -Objekts.

Der Zeit Planerstellungsprozess entspricht der [API-Richtlinie für ressourcenbasierte Vorgänge mit langer Ausführungszeit (relo)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).
Wenn Clients die PUT-Methode verwenden, wird der Zeitplan durch den Vorgang ersetzt, wenn der Zeitplan vorgesehen ist. Andernfalls startet der Vorgang den Zeitplan für die bereitstellen im Hintergrund.

Während der Terminplanung können Clients die [Get-Methode](schedule-get.md) verwenden, um den Zeitplan abzurufen und die `provisionStatus` Eigenschaft für den aktuellen Status der proaktivierung zu überprüfen. Wenn die Einrichtung fehlgeschlagen ist, können Clients zusätzliche Informationen von der `provisionStatusCode` -Eigenschaft abrufen.

Clients können auch die Konfiguration des Zeitplans überprüfen.


## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Group.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Nicht unterstützt |

> **Hinweis**: Diese API unterstützt Administratorberechtigungen. Globale Administratoren können auf Gruppen zugreifen, von denen Sie nicht Mitglied sind.

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule
```

## <a name="request-headers"></a>Anforderungsheader

| Kopfzeile       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext eine JSON-Darstellung eines [Schedule](../resources/schedule.md) -Objekts an.

## <a name="response"></a>Antwort

Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein [Schedule](../resources/schedule.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

#### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "team-put-schedule"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule
Content-type: application/json

{
  "enabled": true,
  "timeZone": "America/Chicago"
}
```

#### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort. 

>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedule"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates or replaces the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/team-put-schedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
