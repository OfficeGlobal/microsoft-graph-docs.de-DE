---
title: AccessReview aktualisieren
description: In Azure AD Access Feature überprüft, und Aktualisieren eines vorhandenen AccessReview-Objekts, um eine oder mehrere Eigenschaften ändern.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1256ccdabea8eb5c0c0ffb3365e0c87276999236
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524366"
---
# <a name="update-accessreview"></a>AccessReview aktualisieren

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aktualisieren Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature eines vorhandenen [AccessReview](../resources/accessreview.md) -Objekts, um eine oder mehrere Eigenschaften ändern.

Diese API ist nicht so ändern Sie die Bearbeiter oder Entscheidungen einer Überprüfung vorgesehen.  Um die Bearbeiter ändern möchten, verwenden Sie die [AddReviewer](accessreview-addreviewer.md) oder [RemoveReviewer](accessreview-removereviewer.md) APIs.  Verwenden Sie eine einmalige Überprüfung bei bereits gestartet, oder eine Instanz bereits gestartet periodische Wiederholung frühzeitig und, um beenden [Beenden](accessreview-stop.md) API. Um die Entscheidungen über die Ziel-Gruppe oder app Zugriffsrechte anwenden möchten, verwenden Sie die [anwenden](accessreview-apply.md) API. 


## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)     | AccessReview.ReadWrite.All |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
|Anwendung                            | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a>Anforderungsheader
| Name         | Typ        | Beschreibung |
|:-------------|:------------|:------------|
| Authorization | string | Bearertoken Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung eine JSON-Darstellung der Parameter eines [AccessReview](../resources/accessreview.md) -Objekts.

In der folgenden Tabelle werden die Eigenschaften gezeigt, die beim Aktualisieren von einer AccessReview bereitgestellt werden können.

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | Der Name des Access überprüfen.  |
| `startDateTime`           |`DateTimeOffset`                                                | Den DateTime-Wert, wenn die Überprüfung geplant ist, gestartet werden.  Dies muss ein Datum in der Zukunft sein.   |
| `endDateTime`             |`DateTimeOffset`                                                | Den DateTime-Wert, wenn die Überprüfung geplant ist, um zu beenden. Dies muss mindestens einen Tag später als das Startdatum sein.   |
| `description`             |`String`                                                        | Die Beschreibung für die Bearbeiter angezeigt. |



## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode eine `204, Accepted` Antwortcode und eines [AccessReview](../resources/accessreview.md) -Objekts in der Antworttext.

## <a name="example"></a>Beispiel

Dies ist ein Beispiel für eine einmalige (nicht wiederkehrenden) Access Überprüfung aktualisieren.

##### <a name="request"></a>Anforderung
Geben Sie im Textkörper Anforderung eine JSON-Darstellung der neuen Eigenschaften des [AccessReview](../resources/accessreview.md) -Objekts.

<!-- {
  "blockType": "request",
  "name": "update_accessReview"
}-->
```http
PATCH https://graph.microsoft.com/beta/accessReviews('006111db-0810-4494-a6df-904d368bd81b')
Content-type: application/json

{
    "displayName":"TestReview new name"
}
```

##### <a name="response"></a>Antwort
>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview new name",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegated",
    "description": "Sample description"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
