# <a name="list-subscriptions"></a>Liste von Abonnements

Rufen Sie die Eigenschaften und Beziehungen von Webhook-Abonnements basierend auf der App-ID, dem Benutzer und der Rolle des Benutzers mit einem Mandanten ab.

## <a name="permissions"></a>Berechtigungen

Diese API unterstützt die folgenden Berechtigungsbereiche. Weitere Informationen, unter anderem dazu, wie Sie Berechtigungen auswählen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).

| Berechtigungstyp  | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)  |
|:---------------- |:-------------------------------------------- |
| [Delegiert](../../../concepts/auth_v2_user.md)(Geschäfts-, Schul- oder Unikonto) | Rolle, die zum [Abonnement erstellen](subscription_get.md) oder für Subscriptions.Read.All  (siehe unten) erforderlich ist. |
| [Delegiert](../../../concepts/auth_v2_user.md) (persönliches Microsoft-Konto) | Rolle, die zum [Abonnement erstellen](./subscription_get.md) oder für Subscriptions.Read.All  (siehe unten) erforderlich ist. |
| [Anwendung](../../../concepts/auth_v2_service.md) | Rolle, die zum [Abonnement erstellen](./subscription_get.md) erforderlich ist. |

Response-Ergebnisse basieren auf dem Kontext der aufrufenden App. Es folgt eine Zusammenfassung der gängigen Szenarien:

### <a name="basic-scenarios"></a>Grundlegende Szenarios

In der Regel möchte eine Anwendung Abonnements abrufen, die sie ursprünglich für den derzeit angemeldeten Benutzer oder für alle Benutzer im Verzeichnis (Geschäfts-/Schul-/Uni-Konten) erstellt hat. Für diese Szenarien sind keine besonderen Berechtigungen erforderlich, die über diejenigen hinausgehen, die ursprünglich von der App zum Erstellen der Abonnements verwendet wurden.

| Kontext der aufrufenden App | Antwort enthält |
|:-----|:---------------- |
| App ruft im Namen des angemeldeten Benutzers auf (delegierte Berechtigung). <br/>-und-<br/>App verfügt über die ursprüngliche Berechtigung, die zum [Abonnement erstellen](subscription_post_subscriptions.md)erforderlich ist.<br/><br/>Hinweis: Dies gilt für persönliche Microsoft-Konten und Geschäfts-/Schul-/Uni-Konten. | Abonnements, die durch **diese App** nur für den angemeldeten Benutzer erstellt werden. |
| App ruft eigenständig auf (Anwendungsberechtigung).<br/>-und-<br/>App verfügt über die ursprüngliche Berechtigung, die zum [Abonnement erstellen](subscription_post_subscriptions.md)erforderlich ist.<br/><br/>Hinweis: Dies gilt nur für Geschäfts-/Schul-/Uni-Konten.| Abonnements, die durch **diese App** für sich oder für einen beliebigen Benutzer im Verzeichnis erstellt werden.|

### <a name="advanced-scenarios"></a>Erweiterte Szenarien

In einigen Fällen möchte eine App Abonnements abrufen, die von anderen Apps erstellt wurden. Beispielsweise möchte ein Benutzer alle Abonnements anzeigen, die von einer beliebigen App eigenständig erstellt wurden. Oder ein Administrator möchte möglicherweise alle Abonnements von allen Apps in deren Verzeichnis sehen.
Für solche Szenarien ist eine delegierte Berechtigung Subscription.Read.All erforderlich.

| Kontext der aufrufenden App | Antwort enthält |
|:-----|:---------------- |
| App ruft im Namen des angemeldeten Benutzers auf (delegierte Berechtigung). *Der Benutzer ist ein Nicht-Administrator*. <br/>-und-<br/>App verfügt über die Berechtigung Subscription.Read.All<br/><br/>Hinweis: Dies gilt für persönliche Microsoft-Konten und Geschäfts-/Schul-/Uni-Konten. | Abonnements, die durch **eine beliebige App** nur für den angemeldeten Benutzer erstellt werden. |
| App ruft im Namen des angemeldeten Benutzers auf (delegierte Berechtigung). *Der Benutzer ist ein Administrator*.<br/>-und-<br/>App verfügt über die Berechtigung Subscription.Read.All<br/><br/>Hinweis: Dies gilt nur für Geschäfts-/Schul-/Uni-Konten. | Abonnements, die durch **eine beliebige App** für **einen beliebigen Benutzer**im Verzeichnis erstellt werden.|

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt nicht die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.

## <a name="request-headers"></a>Anforderungsheader

| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Autorisierung  | Zeichenfolge  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext

Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Bei Erfolg gibt diese Methode im Antworttext einen `200 OK` Antwortcode und eine Liste von [Abonnement](../resources/subscription.md) .-Objekten zurück.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a>Antwort

Es folgt das Beispiel einer Antwort.  Bitte beachten Sie, dass diese aus Platzgründen gekürzt sein kann.  Alle unterstützten Eigenschaften, die für die Anforderung und den Kontext des Aufrufs geeignet sind, werden von einem tatsächlichen Aufruf zurückgegeben.

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 586

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions",
  "value": [
    {
      "id": "0fc0d6db-0073-42e5-a186-853da75fb308",
      "resource": "Users",
      "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
      "changeType": "updated,deleted",
      "clientState": null,
      "notificationUrl": "https://webhookappexample.azurewebsites.net/api/notifications",
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

Gibt eine Anforderung mehrere Seiten mit Daten zurück, enthält die Antwort eine `@odata.nextLink` -Eigenschaft zur einfacheren Verwaltung der Ergebnisse.  Weitere Informationen finden Sie unter [Paging der Microsoft Graph-Daten in Ihrer App](../../../concepts/paging.md).
