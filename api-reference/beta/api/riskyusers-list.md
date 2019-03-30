---
title: RiskyUsers aufListen
description: Ruft die Eigenschaften und Beziehungen eines **riskyUsers** -Objekts ab.
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a902daf00f80470e1ac9a83a287eac507d55e171
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/30/2019
ms.locfileid: "31003727"
---
# <a name="list-riskyusers"></a>RiskyUsers aufListen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ruft die Eigenschaften und Beziehungen eines **riskyUsers** -Objekts ab.

>**Hinweis:** Die Verwendung der riskyUsers-API erfordert eine Azure AD Premium P2-Lizenz.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | IdentityRiskyUser.Read.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | IdentityRiskyUser.Read.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unter `$filter` stützt die Anpassung der Abfrageantwort. Sehen Sie sich das Beispiel weiter unten in diesem Thema an. 

## <a name="request-headers"></a>Anforderungsheader
| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |
| Arbeitsmappensitzungs-ID  | Sitzungs-ID der Arbeitsmappe, die bestimmt, ob Änderungen beibehalten werden. Optional.|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein [identityRiskEvent](../resources/identityriskevent.md) -Objekt im Antworttext zurück.
## <a name="examples"></a>Beispiele
#### <a name="example-1-list-risky-users"></a>Beispiel 1: aufListen von riskanten Benutzern
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```

Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 200 OK
{
  "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "riskLastUpdatedDateTime": "2016-01-29T20:03:57.7872426Z",
  "isGuest": "true",
  "isProcessing": true,
  "isDeleted": "true",
  "riskDetail": "adminConfirmedSigninCompromised",
  "riskLevel": "high",
  "riskState": "atRisk"
  "userDisplayName": "Jon Doe",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
#### <a name="example-2-list-risky-users-and-filter-the-results"></a>Beispiel 2: aufListen von riskanten Benutzern und Filtern der Ergebnisse
Das folgende Beispiel zeigt, wie Sie `$filter` die Auflistung von riskyUser abrufen, deren aggregierte Risikostufe Mittel ist.
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 200 OK
{
      "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
      "riskLastUpdatedDateTime": "2018-09-22T00:04:49.1195968Z",
      "isGuest": false,
      "isProcessing": true,
      "isDeleted": false,
      "riskDetail": "none",
      "riskLevel": "medium",
      "riskState": "atRisk",
      "userDisplayName": "Jon Doe",
      "userPrincipalName": "jon@contoso.com",
      }
    }
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
