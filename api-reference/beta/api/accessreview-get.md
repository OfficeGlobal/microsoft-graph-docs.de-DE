---
title: Abrufen von accessReview
description: 'In Azure AD Access Feature überprüft, ein AccessReview-Objekt abrufen.  '
ms.openlocfilehash: ecd802613e6ab36816800197c00595c90426fb2f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059668"
---
# <a name="get-accessreview"></a>Abrufen von accessReview

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Rufen Sie in der Azure AD [Access überprüft](../resources/accessreviews-root.md) -Funktion ein [AccessReview](../resources/accessreview.md) -Objekt ab.  

Verwenden Sie zum Abrufen der Bearbeiter die Überprüfung Access die [Liste AccessReview Bearbeiter](accessreview-listreviewers.md) API. Verwenden Sie zum Abrufen der Entscheidungen der Access Überprüfung der [Liste AccessReview Entscheidungen](accessreview-listdecisions.md) -API oder der [Liste Meine AccessReview Entscheidungen](accessreview-listmydecisions.md) -API.

Ist dies eine periodische Access-Überprüfung, und verwenden Sie dann die `instances` Beziehung zum Abrufen einer [AccessReview](../resources/accessreview.md) -Auflistung des aktuellen und zukünftigen Instanzen der Access Überprüfung der Vergangenheit.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)     | `AccessReview.Read.All`, `AccessReview.ReadWrite.All`.  Der Benutzer angemeldet muss auch in einer Rolle Directory ermöglicht eine Überprüfung Access lesen oder als ein Prüfer für die Überprüfung Access zugewiesen. |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
|Anwendung                            | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a>Anforderungsheader
| Name         | Typ        | Beschreibung |
|:-------------|:------------|:------------|
| Authorization | string | Bearer \{token\}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Keine Anforderungstext sollte angegeben werden.

## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200, OK` Antwortcode und eines [AccessReview](../resources/accessreview.md) -Objekts in der Antworttext.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')
```

##### <a name="response"></a>Antwort
>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
    "displayName": "review",
    "startDateTime": "2017-11-14T01:14:54.89Z",
    "endDateTime": "2017-12-14T01:14:54.89Z",
    "status": "InProgress",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "self",
    "description": "",
    "settings": {
        "reviewId": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval": true,
        "recurrenceSettings": {
            "recurrenceType": "onetime",
            "recurrenceEndType": "endBy",
            "durationInDays": 0,
            "recurrenceCount": 0
        }
    }
}
```

## <a name="see-also"></a>Siehe auch

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Erstellen von accessReview](accessreview-create.md) |    [accessReview](../resources/accessreview.md) |  Erstellen Sie eine neue AccessReview. |
|[Liste programControls](programcontrol-list.md) | [ProgramControl](../resources/programcontrol.md) -Auflistung | Liste ProgramControls in einem Mandanten. |
|[Liste AccessReview Bearbeiter](accessreview-listreviewers.md) |     [Benutzeridentität](../resources/useridentity.md) -Auflistung|    Rufen Sie die Bearbeiter ein AccessReview. |
|[Liste AccessReview Entscheidungen](accessreview-listdecisions.md) |     [AccessReviewDecision](../resources/accessreviewdecision.md) -Auflistung|    Rufen Sie die Entscheidungen des ein AccessReview.|
|[Meine AccessReview Entscheidungen auflisten](accessreview-listmydecisions.md) |        [AccessReviewDecision](../resources/accessreviewdecision.md) -Auflistung|    Rufen Sie als "Leser" Mein Entscheidungen von einer AccessReview.|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
