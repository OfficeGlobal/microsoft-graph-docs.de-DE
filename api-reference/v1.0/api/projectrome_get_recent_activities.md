# <a name="get-recent-user-activities"></a>Aktuelle Nutzeraktivitäten abrufen

Letzte Aktivitäten für einen bestimmten Benutzer abrufen. Diese OData-Funktion verfügt über einige Standardverhalten, sodass sie wie eine "zuletzt verwendet"-API  ausgeführt wird. Der Dienst fragt die aktuellen [HistoryItems](../resources/projectrome_historyitem.md) ab und zieht diese zugehörigen Aktivitäten. Aktivitäten werden entsprechend der neuesten **lastModified** im **historyItem** sortiert. Dies bedeutet, dass Aktivitäten ohne **historyItems** nicht in der Antwort enthalten sind. Die Berechtigung UserActivity.ReadWrite.CreatedByApp wendet auch eine zusätzliche Filterung für die Antwort an, sodass nur von Ihrer Anwendung erstellte Aktivitäten zurückgegeben werden. Diese serverseitige Filterung kann zu leeren Seiten führen, wenn der Benutzer besonders aktiv ist und andere Anwendungen neuere Aktivitäten erstellt haben. Um die Aktivitäten Ihrer Anwendung abzurufen, verwenden Sie die **NextLink**-Eigenschaft für die Paginierung.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | UserActivity.ReadWrite.CreatedByApp    |
|Delegiert (persönliches Microsoft-Konto) | UserActivity.ReadWrite.CreatedByApp    |
|Anwendung | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort. Die folgenden Abfrageparameter werden unterstützt:

- $expand Sie für die Navigationseigenschaft **historyItems**.
- $top um die maximale Anzahl von Elementen auf mehreren Seiten zu begrenzen.
- $filter auf die **LastModifiedDateTime** -Eigenschaft für **Aktivitäten**  oder ** HistoryItems**, falls erweitert.

Es folgen einige Beispiele für unterstützte Abfragen mit URL-Codierung.

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a>Anforderungsheader

|Name | Typ | Beschreibung|
|:----|:-----|:-----------|
|Autorisierung | Zeichenfolge | Bearer {token}. Erforderlich.|

## <a name="request-body"></a>Anforderungstext

Geben Sie keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode den `200 OK` Antwortcode mit den neuesten Benutzeraktivitäten für ihre Anwendung aus.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.

<!-- {
  "blockType": "request",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities/recent
```

##### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userActivity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.userActivity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "http://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": false,
              },
            "displayText": "Contoso How-To: How to Tie a Reef Knot",
            "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
            "backgroundColor": "#ff0000",
            "content": {
              "$schema": "http://adaptivecards.io/schemas/adaptive-card.json",
              "type": "AdaptiveCard",
              "body":
              [{
                  "type": "TextBlock",
                  "text": "Contoso MainPage"
              }]
            }
        },
        "activationUrl": "http://www.contoso.com/article?id=12345",
        "appDisplayName": "Contoso, Ltd.",
        "userTimezone": "Africa/Casablanca",
        "fallbackUrl": "http://www.contoso.com/article?id=12345",
        "contentUrl": "http://www.contoso.com/article?id=12345",
        "contentInfo": {
            "@context": "http://schema.org",
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
<!-- {
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: get_recent_activities/container/contentInfo:
      Property 'contentInfo' is of type Custom but has no custom members."
  ],
  "tocPath": ""
}-->
