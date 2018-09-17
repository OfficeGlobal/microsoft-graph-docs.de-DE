# <a name="subscription-resource-type"></a>Ressourcentyp Abonnement

Mit einem Abonnement kann eine Client-App Benachrichtigungen zu Änderungen an den Daten in Microsoft Graph erhalten. Abonnements werden derzeit für die folgenden Ressourcen aktiviert:

- E-Mail, Ereignisse und Kontakte aus Outlook
- Unterhaltungen aus Office-Gruppen
- Laufwerkstammelemente aus OneDrive
- Benutzer und Gruppen aus dem Azure Active Directory

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscription",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false,
        "sortable": false
      }
    }
  ]
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------|:-----|:------------|
| changeType | Zeichenfolge | Erforderlich. Gibt den Typ der Änderung in der abonnierten Ressource an, die eine Benachrichtigung auslöst. Unterstützte Werte sind: `created`, `updated`, `deleted`. Es können mehrere Werte mithilfe einer durch Komma getrennten Liste zusammen verwendet werden.<br><br>Hinweis: Laufwerk Stamm-Element Benachrichtigungs-Support unterstützen nur den `updated` ChangeType. Support für Benutzer und Gruppen-Benachrichtigungen `updated` und `deleted` changeType.|
| notificationUrl | Zeichenfolge | Erforderlich. Die URL des Endpunkts, die Benachrichtigungen erhalten werden. Diese URL muss das HTTPS-Protokoll nutzen. |
| Ressource | Zeichenfolge | Erforderlich. Gibt die Ressource ab, die für Änderungen überwacht wird. Die Basis-URL nicht einschließen (`https://graph.microsoft.com/v1.0/`). |
| expirationDateTime | [dateTime](http://tools.ietf.org/html/rfc3339) | Erforderlich. Gibt Datum und Uhrzeit für das Ablaufen des Webhook-Abonnements an. Die Zeit wird in UTC angegeben und kann eine Dauer aus der Erstellung des Abonnements sein, die von der abonnierten Ressource abweicht.  In der folgenden Tabelle finden Sie die maximale Dauer unterstützter Abonnements. |
| clientState | Zeichenfolge | Optional. Gibt den Wert der `clientState`-Eigenschaft an, die in jeder Benachrichtigung vom Dienst gesendet wird. Die Höchstlänge beträgt 128 Zeichen. Der Client kann prüfen, ob die Benachrichtigung vom Dienst stammt, indem er den Wert der mit dem Abonnement gesendeten `clientState`-Eigenschaft mit dem Wert der mit jeder Benachrichtigung empfangenen `clientState`-Eigenschaft vergleicht. |
| ID | Zeichenfolge | Eindeutige ID für das Abonnement. Schreibgeschützt. |
| applicationId | Zeichenfolge | Bezeichner der Anwendung, die verwendet wird, um das Abonnement zu erstellen. Schreibgeschützt. |
| creatorId | Zeichenfolge | Bezeichner des Benutzers oder des Dienstprinzipals, der das Abonnement erstellt hat. Wenn die App zum Erstellen des Abonnements delegierte Berechtigungen verwendet hat, enthält dieses Feld die ID des angemeldeten Nutzers, für den die App im Auftrag von diesem Nutzer angerufen wurde. Wenn die App Anwendungsberechtigungen verwendet hat, enthält dieses Feld die Id des Dienstprinzipals entsprechend der App. Schreibgeschützt. |

## <a name="maximum-length-of-subscription-per-resource-type"></a>Maximale Abonnementdauer pro Ressourcentyp

| Ressource            | Maximal zulässige Ablaufzeit  |
|:--------------------|:-------------------------|
| E-Mail                | 4230 Minuten (unter 3 Tage)    |
| Kalender            | 4230 Minuten (unter 3 Tage)    |
| Kontakte            | 4230 Minuten (unter 3 Tage)    |
| Gruppenunterhaltungen | 4230 Minuten (unter 3 Tage)    |
| Laufwerkstammelemente    | 4230 Minuten (unter 3 Tage)    |

> **Hinweis:** Vorhandene Anwendungen und neue Anwendungen sollten den unterstützten Wert nicht überschreiten. In Zukunft werden alle Anforderungen zum Erstellen oder Erneuern eines Abonnements über den Maximalwert hinaus fehlschlagen.

## <a name="relationships"></a>Beziehungen

Keine

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:-------|:------------|:------------|
| [Abonnement erstellen](../api/subscription_post_subscriptions.md) | [Abonnement](subscription.md) | Abonniert eine Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Microsoft Graph-Daten geändert werden. |
| [Abonnement aktualisieren](../api/subscription_update.md) | [Abonnement](subscription.md) | Erneuert ein Abonnement durch Aktualisierung der Ablaufzeit. |
| [Liste von Abonnements](../api/subscription_list.md) | [Abonnement](subscription.md) | Listen aktiver Abonnements. |
| [Abonnement abrufen](../api/subscription_get.md) | [Abonnement](subscription.md) | Dient zum Lesen der Eigenschaften und der Beziehungen des subscription-Objekts. |
| [Abonnement löschen](../api/subscription_delete.md) | Keine |Löscht ein subscription-Objekt. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
