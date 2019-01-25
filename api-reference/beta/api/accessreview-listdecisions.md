---
title: Liste AccessReview Entscheidungen
description: In Azure AD Access Feature überprüft, die Entscheidungen eines AccessReview-Objekts abrufen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: eeaa1374bbd44cfe9556e488d25e0fc2c7594cde
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521796"
---
# <a name="list-accessreview-decisions"></a>Liste AccessReview Entscheidungen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Abgerufen Sie in der Azure AD [Access überprüft](../resources/accessreviews-root.md) -Funktion werden die Entscheidungen eines [AccessReview](../resources/accessreview.md) -Objekts.

Beachten Sie, dass sich wiederholenden Access Wiederholung wird eine `decisions` Beziehung.  Stattdessen muss der Aufrufer navigieren die `instance` Beziehung zu suchen ein `accessReview` -Objekt für eine aktuelle oder frühere Instanz der Überprüfung Access.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)     | `AccessReview.Read.All`, `AccessReview.ReadWrite.All`.  Der Benutzer angemeldet muss auch in einer Directory-Rolle sein, die diese zum Lesen von einer Überprüfung Zugriff zulässt. |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
|Anwendung                            | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a>Anforderungsheader
| Name         | Typ        | Beschreibung |
|:-------------|:------------|:------------|
| Authorization | string | Bearertoken Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Keine Anforderungstext sollte angegeben werden.

## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200, OK` Antwortcode und ein Array von [AccessReviewDecision](../resources/accessreviewdecision.md) -Objekten im Antworttext.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/decisions
```

##### <a name="response"></a>Antwort
>**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewDecision",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
            "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "accessReviewId": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "reviewResult": "Approve",
            "userPrincipalName": "alice@litware.com",
            "userId": "Alice Smith"
    }
    ]
}
```

## <a name="see-also"></a>Siehe auch

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von accessReview](accessreview-get.md) |  [accessReview](../resources/accessreview.md) |  Abrufen einer Access-Überprüfung. |
|[Meine AccessReview Entscheidungen auflisten](accessreview-listmydecisions.md) |        [AccessReviewDecision](../resources/accessreviewdecision.md) -Auflistung|    Rufen Sie als "Leser" Mein Entscheidungen von einer AccessReview.|
|[AccessReview Erinnerung senden](accessreview-sendreminder.md) |       Keine.   |   Senden Sie eine Erinnerung an die Bearbeiter ein AccessReview. |
|[AccessReview beenden](accessreview-stop.md) |        Keine.   |   Beenden einer AccessReview. |
|[AccessReview Entscheidungen zurücksetzen](accessreview-reset.md) |        Keine.   |   Setzen Sie die Entscheidungen in einer laufenden AccessReview zurück.|
|[Anwenden von AccessReview Entscheidungen](accessreview-apply.md) |        Keine.   |   Gelten Sie die Entscheidungen aus einer abgeschlossenen AccessReview.|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listdecisions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
