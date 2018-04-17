# <a name="mailfolder-resource-type"></a>mailFolder-Ressoucentyp

Ein mailFolder-Element im Postfach eines Benutzers, wie z. B. Posteingang und Entwürfe. Mailordner können Nachrichten, andere Outlook-Elemente und untergeordnete E-Mail-Ordner enthalten.

Outlook erstellt standardmäßig bestimmte Ordner für Benutzer. Anstatt den entsprechenden Ordner-**ID**-Wert zu verwenden, können Sie der Einfachheit halber die folgenden bekannten Ordnernamen beim Zugriff auf diese Ordner in einer **mailFolder**-Sammlung verwenden: `ArchiveRoot`, `ConversationHistory`, `DeletedItems`, `Drafts`, `Inbox`, `JunkEmail`, `Outbox` und `SentItems`.

Diese Ressource unterstützt die Verwendung einer [Delta-Abfrage](../../../concepts/delta_query_overview.md) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen einer [delta](../api/mailfolder_delta.md)-Funktion.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Get mailFolder](../api/mailfolder_get.md) | [mailFolder](mailfolder.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des mailFolder-Objekts.|
|[Create MailFolder](../api/mailfolder_post_childfolders.md) |[MailFolder](mailfolder.md)| Dient zum Erstellen eines neuen mailFolder-Elements unter dem aktuellen durch die Veröffentlichung der childFolders-Sammlung.|
|[List childFolders](../api/mailfolder_list_childfolders.md) |[MailFolder](mailfolder.md)-Sammlung| Dient zum Abrufen der Ordnersammlung unter dem angegebenen Ordner. Sie können die `.../me/MailFolders`Verknüpfung zum Abrufen der Ordnersammlung auf oberster Ebene und zum Navigieren zu einem anderen Ordner verwenden.|
|[Create Message](../api/mailfolder_post_messages.md) |[Nachricht](message.md)| Dient zum Erstellen einer neuen Nachricht in dem aktuellen mailFolder-Element durch die Veröffentlichung in der Nachrichtensammlung.|
|[List messages](../api/mailfolder_list_messages.md) |[Nachrichten](message.md)-Sammlung| Dient zum Abrufen aller Nachrichten im Postfach des angemeldeten Benutzers oder Nachrichten in einen bestimmten Ordner im Postfach.|
|[Update](../api/mailfolder_update.md) | [mailFolder](mailfolder.md)|Dient zum Aktualisieren des angegebenen mailFolder-Objekts. |
|[Delete](../api/mailfolder_delete.md) | Keine |Dient zum Löschen des angegebenen mailFolder-Objekts. |
|[copy](../api/mailfolder_copy.md)|[MailFolder](mailfolder.md)|Dient zum Kopieren eines mailFolder-Elements und seiner Inhalte in ein anderes mailFolder-Element.|
|[delta](../api/mailfolder_delta.md)|[mailFolder](mailfolder.md)-Sammlung|Dient zum Abrufen eines Satzes von E-Mail-Ordnern, die dem Postfach des Benutzers hinzugefügt bzw. daraus gelöscht oder entfernt wurden.|
|[move](../api/mailfolder_move.md)|[MailFolder](mailfolder.md)|Dient zum Verschieben eines mailFolder-Elements und seiner Inhalte in ein anderes mailFolder-Element.|
|[Create single-value extended property](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[mailFolder](mailFolder.md)  |Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen mailFolder-Element.   |
|[Get mailFolder with single-value extended property](../api/singlevaluelegacyextendedproperty_get.md)  | [mailFolder](mailFolder.md) | Dient zum Abrufen von mailFolders-Elementen mit einer erweiterten einwertigen Eigenschaft mithilfe von `$expand` oder `$filter`. |
|[Create multi-value extended property](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [mailFolder](mailFolder.md) | Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen mailFolder-Element.  |
|[Get mailFolder with multi-value extended property](../api/multivaluelegacyextendedproperty_get.md)  | [mailFolder](mailFolder.md) | Dient zum Abrufen eines mailFolders-Elements mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|childFolderCount|Int32|Die Anzahl der unmittelbar untergeordneten mailFolders-Elemente in dem aktuellen mailFolder-Element.|
|displayName|String|Der Anzeigename des mailFolder-Elements.|
|id|String|Der eindeutiger Bezeichner des mailFolder-Elements. Sie können die folgenden häufig verwendeten Bezeichnungen für den Zugriff auf den entsprechenden Ordner verwenden: Posteingang, Entwürfe, Gesendete Elemente, DeletedItems.|
|parentFolderId|String|Die eindeutige ID für das übergeordnete mailFolder-Element des mailFolder-Elements.|
|totalItemCount|Int32|Anzahl der Elemente im mailFolder-Element.|
|unreadItemCount|Int32|Die Anzahl der Elemente im mailFolder-Element, die als „Ungelesen“ markiert sind.|

**Effizientes Ermitteln der Anzahl von Elementen**

Mit den TotalItemCount- und UnreadItemCount-Eigenschaften eines Ordners können Sie die Anzahl der gelesenen Elemente im Ordner problemlos ermitteln. Mithilfe dieser Eigenschaften werden Abfragen folgender Art vermieden, die zu erheblichen Wartezeiten führen:
```
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```
MailFolders-Elemente in Outlook können mehr als einen Typ von Elementen enthalten, der Posteingang kann beispielsweise Besprechungsanfragen enthalten, die sich von E-Mail-Elementen unterscheiden. TotalItemCount und UnreadItemCount schließen Elemente in einem mailFolder-Element unabhängig von Elementtyp ein.


## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|childFolders|[MailFolder](mailfolder.md)-Sammlung|Die Sammlung der untergeordneten Ordner in dem mailFolder-Element.|
|messageRules | [messageRule](messagerule.md)-Sammlung | Die Sammlung von Regeln, die für den Posteingangsordner des Benutzers gelten. | 
|Nachrichten|[Nachrichten](message.md)-Sammlung|Die Sammlung der Nachrichten in dem mailFolder-Element.|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung| Die Sammlung erweiterter mehrwertiger Eigenschaften, die für das mailFolder-Element definiert sind. Schreibgeschützt. Lässt Nullwerte zu.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung| Die Sammlung erweiterter einwertiger Eigenschaften, die für das mailFolder-Element definiert sind. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules", 
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailFolder"
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024,

  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}

```

## <a name="see-also"></a>Siehe auch

- [Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten](../../../concepts/delta_query_overview.md)
- [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](../../../concepts/delta_query_messages.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
