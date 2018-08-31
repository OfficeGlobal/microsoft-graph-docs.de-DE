# <a name="attendeebase-resource-type"></a>Ressourcentyp „attendeeBase“

Der Typ eines Teilnehmers.

Abgeleitet von [recipient](recipient.md).

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.recipient",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|type|attendeeType| Der Typ eines Teilnehmers. Mögliche Werte sind `required`, `optional`,`resource`. Hinweis: Wenn der Teilnehmer eine Person ist, berücksichtigt [FindMeetingTimes](../api/user_findmeetingtimes.md) immer, dass die Person vom `Required`-Typ ist.|
|emailAddress|[emailAddress](emailAddress.md)|Enthält den Namen und die SMTP-Adresse des Teilnehmers.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
