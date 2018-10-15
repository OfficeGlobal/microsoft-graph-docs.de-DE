# <a name="mailfolder-resource-type"></a>mailFolder-Ressoucentyp

Ein mailFolder-Element im Postfach eines Benutzers, wie z. B. Posteingang und Entwürfe. Mailordner können Nachrichten, andere Outlook-Elemente und untergeordnete Mail-Ordner enthalten.

Diese Ressource unterstützt die Verwendung einer [Delta-Abfrage](../../../concepts/delta_query_overview.md) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen einer [delta](../api/mailfolder_delta.md)-Funktion.

**Bekannte Ordnernamen**

Outlook erstellt standardmäßig bestimmte Ordner für Benutzer. Statt den **ID-** Wert des entsprechenden Ordners zu nutzen, können Sie der Einfachheit halber zu diesem Zweck die bekannten Ordnernamen aus der folgenden Tabelle beim Zugriff auf diese Ordner nutzen. Beispielsweise können Sie den Ordner "Entwürfe" unter Verwendung seines bekannten Namens mit der folgenden Abfrage abrufen.

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

Bekannte Namen arbeiten unabhängig von dem Gebietsschema des Postfachs des Benutzers, daher wird die oben genannte Abfrage immer den Ordner „Entwürfe“ des Benutzers, unabhängig davon, wie er heißt, zurückgeben.

| Bekannter Ordnername | Beschreibung |
|:-----------------------|:------------|
| archivieren | Bei Verwendung des One_Click Archiv-Features in Outlook-Clients, die dies unterstützen, werden die Archiv Nachrichten-Ordner gesendet. **Hinweis:** Dies ist nicht das gleiche wie das Archivpostfach Feature von Exchange online. |
| Clutter | Die Nachrichten des Clutter-Ordners mit niedriger Priorität werden verschoben, wenn das Clutter-Feature benutzt wird. |
| Konflikte | Der Ordner, der miteinander in Konflikt stehende Elemente im Postfach enthält. |
| conversationhistory | Der Ordner, in dem Skype IM Unterhaltungen speichert (falls Skype dafür konfiguriert ist). |
| deleteditems | Der Ordner, in den Elemente verschoben werden, wenn sie gelöscht werden. |
| drafts | Der Ordner, der nicht gesendete Nachrichten enthält. |
| inbox | Der Ordner Posteingang. |
| junkemail | Der Junk-e-Mail-Ordner. |
| localfailures | Der Ordner, der Elemente enthält, die auf dem lokalen Client vorhanden sind, jedoch nicht auf den Server hochgeladen werden konnte. |
| msgfolderroot | Der Ordner "Oberste Ebene des Informationsspeichers". Dieser Ordner ist der übergeordnete Ordner für Ordner, die in den normalen Mail-Clients, wie beispielsweise dem Posteingang, angezeigt werden. |
| Postausgang | Der Ordner Postausgang. |
| recoverableitemsdeletions | Der Ordner, der vorläufig gelöschte Elemente enthält: gelöscht entweder aus dem Ordner Gelöschte Objekte oder durch Drücken von UMSCHALT + ENTF in Outlook. Dieser Ordner ist nicht in allen Outlook E-Mail-Clients sichtbar, jedoch können Endbenutzer über das Feature **Gelöschte Elemente vom Server wiederherstellen** in Outlook oder Outlook im Web mit ihm interagieren. |
| scheduled | Der Ordner, der Nachrichten enthält, die im Posteingang mit dem Zeitplan-Feature in Outlook für iOS angezeigt werden sollen. |
| searchfolders | Der übergeordnete Ordner für alle im Postfach des Benutzers definierten Suchordner. |
| sentitems | Der Ordner 'Gesendete Elemente'. |
| serverfailures | Der Ordner, der Elemente enthält, die auf dem Server vorhanden sind, aber nicht mit dem lokalen Client synchronisiert werden konnten. |
| syncissues | Der Ordner, der die von Outlook erstellten Synchronisierungsprotokolle enthält. |

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:-------|:------------|:------------|
|[Get mailFolder](../api/mailfolder_get.md) | [mailFolder](mailfolder.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des mailFolder-Objekts.|
|[MailFolder erstellen](../api/mailfolder_post_childfolders.md) |[MailFolder](mailfolder.md)| Dient zum Erstellen eines neuen mailFolder-Elements unter dem aktuellen durch die Veröffentlichung der childFolders-Sammlung.|
|[Liste der childFolders](../api/mailfolder_list_childfolders.md) |[MailFolder](mailfolder.md)-Sammlung| Dient zum Abrufen der Ordnersammlung unter dem angegebenen Ordner. Sie können die `.../me/MailFolders`Verknüpfung zum Abrufen der Ordnersammlung auf oberster Ebene und zum Navigieren zu einem anderen Ordner verwenden.|
|[Nachricht erstellen](../api/mailfolder_post_messages.md) |[Nachricht](message.md)| Dient zum Erstellen einer neuen Nachricht in dem aktuellen mailFolder-Element durch die Veröffentlichung in der Nachrichtensammlung.|
|[Nachrichten-Liste](../api/mailfolder_list_messages.md) |[Nachrichten](message.md)-Sammlung| Dient zum Abrufen aller Nachrichten im Postfach des angemeldeten Benutzers oder Nachrichten in einen bestimmten Ordner im Postfach.|
|[Aktualisieren](../api/mailfolder_update.md) | [mailFolder](mailfolder.md)|Dient zum Aktualisieren des angegebenen mailFolder-Objekts. |
|[Löschen](../api/mailfolder_delete.md) | Keine |Dient zum Löschen des angegebenen mailFolder-Objekts. |
|[Kopie](../api/mailfolder_copy.md)|[MailFolder](mailfolder.md)|Dient zum Kopieren eines mailFolder-Elements und seiner Inhalte in ein anderes mailFolder-Element.|
|[Delta](../api/mailfolder_delta.md)|[mailFolder](mailfolder.md)-Sammlung|Dient zum Abrufen eines Satzes von E-Mail-Ordnern, die dem Postfach des Benutzers hinzugefügt bzw. daraus gelöscht oder entfernt wurden.|
|[move](../api/mailfolder_move.md)|[MailFolder](mailfolder.md)|Dient zum Verschieben eines mailFolder-Elements und seiner Inhalte in ein anderes mailFolder-Element.|
|**Erweiterte Eigenschaften**| | |
|[Einwertige erweiterte Eigenschaft erstellen](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[mailFolder](mailFolder.md)  |Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen mailFolder-Element.   |
|[MailFolder mit erweiterter Eigenschaft zum Einzelwert anfordern](../api/singlevaluelegacyextendedproperty_get.md)  | [mailFolder](mailFolder.md) | Dient zum Abrufen von mailFolders-Elementen mit einer erweiterten einwertigen Eigenschaft mithilfe von `$expand` oder `$filter`. |
|[Mehrwertige erweiterte Eigenschaft erstellen](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [mailFolder](mailFolder.md) | Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen mailFolder-Element.  |
|[MailFolder mit mehrwertiger erweiterter Eigenschaft anfordern](../api/multivaluelegacyextendedproperty_get.md)  | [mailFolder](mailFolder.md) | Dient zum Abrufen eines mailFolders-Elements mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`. |

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------|:-----|:------------|
|childFolderCount|Int32|Die Anzahl der unmittelbar untergeordneten mailFolders-Elemente in dem aktuellen mailFolder-Element.|
|displayName|Zeichenfolge|Der Anzeigename des mailFolder-Elements.|
|id|Zeichenfolge|Eindeutiger Bezeichner der MailFolder.|
|parentFolderId|Zeichenfolge|Die eindeutige ID für das übergeordnete mailFolder-Element des mailFolder-Elements.|
|totalItemCount|Int32|Anzahl der Elemente im mailFolder-Element.|
|unreadItemCount|Int32|Die Anzahl der Elemente im mailFolder-Element, die als „Ungelesen“ markiert sind.|

**Effizientes Ermitteln der Anzahl von Zugangs-Elementen**

Die `TotalItemCount` und `UnreadItemCount` Eigenschaften eines Ordners ermöglichen es, bequem die Anzahl der gelesenen Elemente im Ordner zu berechnen.
Mithilfe dieser Eigenschaften werden Abfragen folgender Art vermieden, die zu erheblichen Wartezeiten führen:

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

Mail-Ordner in Outlook können mehr als einen Typ von Elementen enthalten; der Posteingang kann beispielsweise Besprechungsanfragen enthalten, die sich von E-Mail-Elementen unterscheiden. `TotalItemCount` und `UnreadItemCount` schließen Elemente in einem Mail-Ordner unabhängig von Elementtyp ein.

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ | Beschreibung |
|:-------------|:-----|:------------|
|childFolders|[MailFolder](mailfolder.md)-Sammlung|Die Sammlung der untergeordneten Ordner in dem mailFolder-Element.|
|messageRules | [messageRule](messagerule.md)-Sammlung | Die Sammlung von Regeln, die für den Posteingangsordner des Benutzers gelten. |
|Nachrichten|[Nachrichten](message.md)-Sammlung|Die Sammlung der Nachrichten in dem mailFolder-Element.|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung| Die Sammlung erweiterter mehrwertiger Eigenschaften, die für das mailFolder-Element definiert sind. Schreibgeschützt. Lässt Nullwerte zu.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung| Die Sammlung erweiterter einwertiger Eigenschaften, die für das mailFolder-Element definiert sind. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.mailFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "changeTracking": false,
        "navigability": "single",
        "searchable": false
      }
    },
    {
      "property": "messageRules",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single"
      }
    }
  ]
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
