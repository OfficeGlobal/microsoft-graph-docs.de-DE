# <a name="post-resource-type"></a>Beitragsressourcentyp
Stellt ein einzelnes Post-Element in einer [conversationThread](conversationthread.md)-Entität dar.

Zwar können Sie Beiträge nicht explizit erstellen; es wird jedoch bei jedem der folgenden Vorgänge ein Beitrag erstellt:

- [auf einen vorhandenen Beitrag antworten](../api/post_reply.md) 
- [auf einen vorhandenen Thread antworten](../api/conversationthread_reply.md) 
- [einen Thread in einer neuen Unterhaltung erstellen](../api/group_post_threads.md)
- [eine neue Unterhaltung erstellen](../api/group_post_conversations.md)

Diese Ressource ermöglicht es Ihnen, benutzerdefinierten Eigenschaften mithilfe von [Erweiterungen](../../../concepts/extensibility_overview.md) eigene Daten hinzuzufügen.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Liste der Beiträge](../api/conversationthread_list_posts.md) | [Beitrag](post.md) |Dient zum Abrufen der Beiträge des angegebenen Threads. |
|[Beitrag anfordern](../api/post_get.md) | [Beitrag](post.md) |Dient zum Abrufen der Eigenschaften und der Beziehungen eines Beitrags in einem angegebenen Thread.|
|[Antwort](../api/post_reply.md)|Keine|Dient zum Antworten auf einen Beitrag und zum Hinzufügen eines neuen Beitrags zum angegebenen Thread in einer Gruppenunterhaltung.|
|[Weiterleiten](../api/post_forward.md)|Keine|Dient zum Weiterleiten eines Beitrags an einen Empfänger.|
|**Anlagen**| | |
|[Liste der Anlagen](../api/post_list_attachments.md) |[Anlagen](attachment.md)-Sammlung| Ruft alle Anlagen für einen Beitrag ab.|
|[Hinzufügen von Anlagen](../api/post_post_attachments.md) |[Anlage](attachment.md)| Dient zum Hinzufügen einer Anlage zu einem Beitrag. |
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Ruft ein offenes Erweiterungsobjekt oder Objekte basierend auf ihrem Namen oder vollqualifizierten Namen ab.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](../../../concepts/extensibility_schema_groups.md) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|
|**Erweiterte Eigenschaften**| | |
|[Einwertige erweiterte Eigenschaft erstellen](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[Beitrag](post.md)  |Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen Beitrag.   |
|[Beitrag mit erweiterter Eigenschaft zum Einzelwert anfordern](../api/singlevaluelegacyextendedproperty_get.md)  | [Beitrag](post.md) | Dient zum Abrufen von Beiträgen mit einer erweiterten einwertigen Eigenschaft mithilfe von `$expand` oder `$filter`. |
|[Mehrwertige erweiterte Eigenschaft erstellen](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [Beitrag](post.md) | Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen Beitrag  |
|[Beiterag mit mehrwertiger erweiterter Eigenschaft anfordern](../api/multivaluelegacyextendedproperty_get.md)  | [Beitrag](post.md) | Dient zum Abrufen eines Beitrags mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Text|[itemBody](itembody.md)|Der Inhalt des Beitrags. Dies ist eine Standardeigenschaft. Für diese Eigenschaft sind Nullwerte zulässig.|
|Kategorien|Zeichenfolgenauflistung|Die Kategorien, die mit dem Beitrag verknüpft sind.|
|changeKey|Zeichenfolge|Gibt die Version des Beitrags an. Jedes Mal, wenn der Beitrag geändert wird, wird auch ChangeKey geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen.|
|conversationId|Zeichenfolge|Eindeutige ID der Unterhaltung. Schreibgeschützt.|
|conversationThreadId|Zeichenfolge|Eindeutige ID des Unterhaltungsthreads. Schreibgeschützt.|
|createdDateTime|DateTimeOffset|Gibt an, wann der Beitrag erstellt wurde. Der DateTimeOffset-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|Von|[Empfänger](recipient.md)|Wird in Zugriffsszenarien mit Stellvertretungen verwendet. Gibt an, wer die Nachricht im Auftrag eines anderen Benutzers veröffentlicht hat. Dies ist eine Standardeigenschaft.|
|hasAttachments|boolesch|Gibt an, ob der Beitrag mindestens eine Anlage enthält. Dies ist eine Standardeigenschaft.|
|ID|Zeichenfolge| Schreibgeschützt.|
|lastModifiedDateTime|DateTimeOffset|Gibt an, wann der Beitrag zuletzt geändert wurde. Der DateTimeOffset-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|newParticipants|[Empfänger](recipient.md)-Sammlung|Teilnehmer einer Unterhaltung, die im Rahmen des Beitrags zu dem Thread hinzugefügt wurden.|
|receivedDateTime|DateTimeOffset|Gibt an, wann der Beitrag empfangen wurde. Der DateTimeOffset-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|Sender|[Empfänger](recipient.md)|Enthält die E-Mail-Adresse des Absenders. Bei dem Sender-Wert wird davon ausgegangen, dass dies die Adresse des authentifizierten Benutzers ist, wenn Absender nicht angegeben wurde. Dies ist eine Standardeigenschaft.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Anlagen|[Anlagensammlung](attachment.md)| Schreibgeschützt. Lässt Nullwerte zu.|
|Erweiterungen|[Erweiterungssammlung](extension.md)|Die Sammlung der für den Beitrag definierten offenen Erweiterungen. Schreibgeschützt. Lässt Nullwerte zu.|
|inReplyTo|[Beitrag](post.md)| Schreibgeschützt.|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung| Die Sammlung erweiterter mehrwertiger Eigenschaften, die für den Beitrag definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung| Die Sammlung erweiterter einwertiger Eigenschaften, die für den Beitrag definiert sind. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "attachments",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "baseType": "microsoft.graph.outlookItem",
  "@odata.type": "microsoft.graph.post",
  "@odata.annotations": [
    {
      "property": "attachments",
      "capabilities": {
        "changeTracking": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "inReplyTo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["string"],
  "changeKey": "string",
  "conversationId": "string",
  "conversationThreadId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "newParticipants": [{"@odata.type": "microsoft.graph.recipient"}],
  "receivedDateTime": "String (timestamp)",
  "sender": {"@odata.type": "microsoft.graph.recipient"}
}

```

## <a name="see-also"></a>Siehe auch

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](../../../concepts/extensibility_overview.md)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](../../../concepts/extensibility_open_users.md)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
