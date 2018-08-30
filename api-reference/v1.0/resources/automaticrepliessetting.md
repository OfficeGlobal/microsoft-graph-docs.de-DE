# <a name="automaticrepliessetting-resource-type"></a>Ressourcentyp automaticRepliesSetting

Konfigurationseinstellungen zum automatischen Benachrichtigen des Absenders bei eingehenden E-Mails mit einer Nachricht vom angemeldeten Benutzer. Beispiel: eine automatische Antwort, die darüber informiert, dass der angemeldete Benutzer zur Beantwortung von E-Mails nicht verfügbar ist. 


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|externalAudience|ExternalAudienceScope| Die Benutzergruppe außerhalb der Organisation des angemeldeten Benutzers, der die **ExternalReplyMessage** erhält, wenn der **Status** `AlwaysEnabled` oder `Scheduled` ist. Mögliche Werte sind: `none`, `contactsOnly`, `all`.|
|externalReplyMessage|Zeichenfolge|Die automatische Antwort an die angegebene externe Zielgruppe, wenn **Status** `AlwaysEnabled` oder `Scheduled` ist.|
|internalReplyMessage|Zeichenfolge|Die automatische Antwort an die interne Zielgruppe in der Organisation des angemeldeten Benutzers, wenn **Status** `AlwaysEnabled` oder `Scheduled` ist. |
|scheduledEndDateTime|[dateTimeTimeZone](datetimetimezone.md)|Datum und Uhrzeit, die zum Beenden der automatischen Antworten festgelegt werden, wenn **Status** auf `Scheduled` gesetzt ist. |
|scheduledStartDateTime|[dateTimeTimeZone](datetimetimezone.md)|Datum und Uhrzeit, die für den Beginn der automatischen Antworten festgelegt werden, wenn **Status** auf `Scheduled` gesetzt ist.|
|Status|AutomaticRepliesStatus|Status der Konfigurationen für automatische Antworten. Mögliche Werte sind: `disabled`, `alwaysEnabled`, `scheduled`.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}-->

```json
{
  "externalAudience": "String",
  "externalReplyMessage": "string",
  "internalReplyMessage": "string",
  "scheduledEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
