---
title: Abrufen aktueller Benutzeraktivitäten
description: " API. Der Dienst für die aktuelle HistoryItems Abfragen, und ziehen Sie die zugehörigen Aktivitäten. Aktivitäten werden entsprechend der neuesten **LastModified** auf die **HistoryItem**sortiert. Dies bedeutet, dass Aktivitäten ohne **HistoryItems** nicht in der Antwort enthalten sein werden. Die Berechtigung UserActivity.ReadWrite.CreatedByApp wird auch gelten zusätzliche Filter auf die Antwort, damit nur Aktivitäten, die von der Anwendung erstellt zurückgegeben werden. Diese serverseitige Filterung auftreten auf leere Seiten, wenn der Benutzer besonders aktiv ist und anderen Applikationen neuere Aktivitäten erstellt haben. Wenn Sie Ihre Anwendung Aktivitäten erhalten möchten, verwenden Sie die **NextLink** -Eigenschaft für die Paginierung."
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 5ac5522472404e70f07b5b658e404cd4e77bbf88
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643958"
---
# <a name="get-recent-user-activities"></a>Abrufen aktueller Benutzeraktivitäten

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Rufen Sie aktuelle Aktivitäten für einen bestimmten Benutzer. Diese OData-Funktion verfügt über einige Standardverhalten enthalten, sodass sie wie eine API "zuletzt verwendet" ausgeführt werden. Der Dienst für die aktuelle [HistoryItems](../resources/projectrome-historyitem.md)Abfragen, und ziehen Sie die zugehörigen Aktivitäten. Aktivitäten werden entsprechend der neuesten **LastModified** auf die **HistoryItem**sortiert. Dies bedeutet, dass Aktivitäten ohne **HistoryItems** nicht in der Antwort enthalten sein werden. Die Berechtigung UserActivity.ReadWrite.CreatedByApp wird auch gelten zusätzliche Filter auf die Antwort, damit nur Aktivitäten, die von der Anwendung erstellt zurückgegeben werden. Diese serverseitige Filterung auftreten auf leere Seiten, wenn der Benutzer besonders aktiv ist und anderen Applikationen neuere Aktivitäten erstellt haben. Wenn Sie Ihre Anwendung Aktivitäten erhalten möchten, verwenden Sie die **NextLink** -Eigenschaft für die Paginierung.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | UserActivity.ReadWrite.CreatedByApp    |
|Delegiert (persönliches Microsoft-Konto) | UserActivity.ReadWrite.CreatedByApp    |
|Application | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt einige [OData-Abfrage-Parameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , mit denen die Antwort anpassen. Die folgenden Abfrageparameter werden unterstützt:

- $ Erweitern Sie für die Eigenschaft **HistoryItems** Navigation.
- $top um die maximale Anzahl von Elementen auf mehreren Seiten zu begrenzen.
- $filter auf die **LastModifiedDateTime** -Eigenschaft für **Aktivitäten** oder **HistoryItems**, wenn erweitert.

Es folgen einige Beispiele für unterstützte Abfragen mit URL-Codierung.

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a>Anforderungsheader

|Name | Typ | Beschreibung|
|:----|:-----|:-----------|
|Autorisierung | string | Bearer {token}. Erforderlich.|

## <a name="request-body"></a>Anforderungstext

Geben Sie einen Anforderungstext nicht.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode die `200 OK` Antwortcode mit den aktuellsten Aktivitäten des Benutzers, für die Anwendung.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.

<!-- {
  "blockType": "ignored",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities/recent
```

##### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.activity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "https://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": "false",
              },
            "displayText": "Contoso How-To: How to Tie a Reef Knot",
            "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
            "backgroundColor": "#ff0000",
            "content": {
              "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
              "type": "AdaptiveCard",
              "body":
              [{
                  "type": "TextBlock",
                  "text": "Contoso MainPage"
              }]
            }
        },
        "activationUrl": "https://www.contoso.com/article?id=12345",
        "appDisplayName": "Contoso, Ltd.",
        "userTimezone": "Africa/Casablanca",
        "fallbackUrl": "https://www.contoso.com/article?id=12345",
        "contentUrl": "https://www.contoso.com/article?id=12345",
        "contentInfo": {
            "@context": "https://schema.org",
            "@type": "Article",
            "author": "John Doe",
            "name": "How to Tie a Reef Knot"
        },
        "expirationDateTime": "2018-03-28T18:34:29.607Z",
        "status": "updated"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-get-recent-activities.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
