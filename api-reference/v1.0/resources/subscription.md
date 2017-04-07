# <a name="subscription-resource-type"></a>Abonnementressourcentyp
Mit einem Abonnement kann eine Client-App Benachrichtigungen zu Daten in Microsoft Graph erhalten. Für die folgenden Datensätze sind derzeit Abonnements aktiviert:

1. E-Mail, Ereignisse und Kontakte aus Outlook
1. Unterhaltungen aus Office-Gruppen.
1. Laufwerkstammelemente aus OneDrive 


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscription"
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|changeType|string|Gibt den Typ der Änderung in der abonnierten Ressource an, die eine Benachrichtigung auslöst. Unterstützte Werte sind: `created`, `updated`, `deleted`. Es können mehrere Werte mithilfe einer durch Trennzeichen getrennten Liste zusammen verwendet werden.|
|notificationUrl|string|Die URL des Endpunkts, der die Benachrichtigungen erhält. Diese URL muss das HTTPS-Protokoll verwenden.|
|Ressourcen|string|Gibt die Ressource an, deren Änderungen überwacht werden. Schließen Sie die Basis-URL nicht mit ein („https://graph.microsoft.com/v1.0/“).|
|expirationDateTime|[dateTime](http://tools.ietf.org/html/rfc3339)|Gibt Datum und Uhrzeit für das Ablaufen des Webhook-Abonnements an. Die Zeit wird in UTC angegeben und kann eine Dauer aus der Erstellung des Abonnements sein, die von der abonnierten Ressource abweicht.  Maximal zulässige Werte finden Sie in der unten aufgeführten Tabelle.|
|clientState|string|Gibt den Wert der `clientState`-Eigenschaft an, die in jeder Benachrichtigung vom Dienst gesendet wird. Die Höchstlänge beträgt 128 Zeichen. Der Client kann prüfen, ob die Benachrichtigung vom Dienst stammt, indem er den Wert der mit dem Abonnement gesendeten `clientState`-Eigenschaft mit dem Wert der mit jeder Benachrichtigung empfangenen `clientState`-Eigenschaft vergleicht.|
|id|string|Eindeutige ID für das Abonnement. Schreibgeschützt.|

## <a name="maximum-expiration-times-per-resource"></a>Maximal zulässige Ablaufzeit pro Ressource
| Ressource | Maximal zulässige Ablaufzeit |
|:---------------------|:--------------------|
|Mail| 4230 Minuten.|
|Kalender| 4230 Minuten.|
|Kontakte| 4230 Minuten.|
|Gruppenunterhaltungen| 4230 Minuten.|
|Laufwerkstammelemente| 86400 Minuten.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Create subscription](../api/subscription_post_subscriptions.md) | [Abonnement](subscription.md) |Abonniert eine Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Microsoft Graph-Daten geändert werden.|
|[Update subscription](../api/subscription_update.md) | [Abonnement](subscription.md) |Erneuert ein Abonnement durch Aktualisierung der Ablaufzeit.|
|[Get subscription](../api/subscription_get.md) | [Abonnement](subscription.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des subscription-Objekts.|
|[Delete subscription](../api/subscription_delete.md) | Keine |Löscht ein subscription-Objekt.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
