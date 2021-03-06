---
title: Nachrichtenressourcentyp
description: Eine Nachricht in einem Postfachordner.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 487427e13d06bc703728986505de789aab65963f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166794"
---
# <a name="message-resource-type"></a>Nachrichtenressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Eine Nachricht in einem Postfachordner.

Diese Ressource unterstützt Folgendes:

- Hinzufügen Ihrer eigenen Daten als benutzerdefinierte Internet-Nachrichtenkopfzeilen. Hinzufügen von benutzerdefinierten Kopfzeilen nur beim Erstellen einer Nachricht und Zuweisen eines mit „x-“ beginnenden Namens. Nachdem die Nachricht gesendet wurde, können Sie die Kopfzeilen nicht ändern. Um die Kopfzeilen einer Nachricht abzurufen, wenden Sie den Abfrageparameter `$select` in einem [get message](../api/message-get.md)-Vorgang an.
- Hinzufügen Ihrer eigenen Daten zu benutzerdefinierten Eigenschaften als [Erweiterungen](/graph/extensibility-overview).
- Abonnieren von [Änderungsbenachrichtigungen](/graph/webhooks).
- Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/message-delta.md)-Funktion.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "extensions",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties",
    "mentions",

    "internetMessageHeaders"
  ],
  "@odata.type": "microsoft.graph.message"
}-->

```json
{
  "bccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "changeKey": "string",
  "conversationId": "string",
  "conversationIndex": "binary",
  "createdDateTime": "String (timestamp)",
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageHeaders": [{"@odata.type": "microsoft.graph.internetMessageHeader"}],
  "internetMessageId": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "mentionsPreview": {"@odata.type": "microsoft.graph.mentionsPreview"},
  "parentFolderId": "string",
  "receivedDateTime": "String (timestamp)",
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "unsubscribeData": "string",
  "unsubscribeEnabled": true,
  "webLink": "string",

  "attachments": [{"@odata.type": "microsoft.graph.attachment"}],
  "extensions": [{"@odata.type": "microsoft.graph.extension"}],
  "mentions": [{"@odata.type": "microsoft.graph.mention"}],
  "multiValueExtendedProperties": [{"@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"}],
  "singleValueExtendedProperties": [{"@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"}]
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|bccRecipients|[recipient](recipient.md) collection|Die Bcc:-Empfänger der Nachricht.|
|body|[itemBody](itembody.md)|Der Text der Nachricht. Er kann im HTML- oder Textformat vorliegen. Weitere Informationen zu [sicherem HTML-Code in einem Nachrichtentext](/graph/outlook-create-send-messages#reading-messages-with-control-over-the-body-format-returned).|
|bodyPreview|String|Die ersten 255 Zeichen des Nachrichtentexts. Liegt im Textformat vor. Wenn die Nachricht Instanzen von [mention](mention.md) enthält, würde diese Eigenschaft auch eine Verkettung dieser Erwähnungen enthalten. |
|categories|String collection|Die Kategorien, die mit der Nachricht verknüpft sind. Jeder Kategorie entspricht der **displayName**-Eigenschaft einer für den Benutzer definierten [outlookCategory](outlookcategory.md). |
|ccRecipients|[recipient](recipient.md) collection|Die Cc:-Empfänger der Nachricht.|
|changeKey|String|Die Version der Nachricht.|
|conversationId|String|Die ID der Unterhaltung, zu der die E-Mail gehört.|
|conversationIndex|Binär|Der Index der Unterhaltung, zu der die E-Mail gehört.|
|createdDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht erstellt wurde.|
|Flag|[followupFlag](followupflag.md)|Der Wert des Flags, der den Status, das Startdatum, das Fälligkeitsdatum oder das Enddatum für die Nachricht angibt.|
|Von|[Empfänger](recipient.md)|Der Postfachbesitzer und Absender der Nachricht. Der Wert muss dem tatsächlich verwendeten Postfach entsprechen. Weitere Informationen über das [Festlegen der Eigenschaften „from“ und „sender“](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) einer Nachricht.|
|hasAttachments|Boolescher Wert|Gibt an, ob die Nachricht Anlagen enthält. Diese Eigenschaft enthält keine Inline-Anlagen, wenn eine Nachrichtalso  nur Inline-Anlagen enthält, ist diese Eigenschaft „false“. Um das Vorhandensein von Inline-Anlagen zu überprüfen, analysieren Sie die **body**-Eigenschaft so, dass nach einem `src`-Attribut, z. B. `<IMG src="cid:image001.jpg@01D26CD8.6C05F070">`, gesucht wird. |
|id|String|Eindeutiger Bezeichner für die Nachricht (beachten Sie, dass sich dieser Wert ändern kann, wenn eine Nachricht verschoben oder geändert wird)|
|Wichtigkeit|String| Wichtigkeit der Nachricht: `Low`, `Normal`, `High`.|
|inferenceClassification|Zeichenfolge| Die Klassifizierung der Nachricht für den Benutzer, basierend auf der abgeleiteten Relevanz oder Wichtigkeit oder auf einer expliziten Außerkraftsetzung. Mögliche Werte sind: `focused`, `other`.|
|internetMessageHeaders | [internetinternetMessageHeaders](internetmessageheader.md)-Sammlung | Eine Sammlung von Nachrichtenkopfzeilen, definiert von [RFC5322](https://www.ietf.org/rfc/rfc5322.txt). Der Satz enthält Nachrichtenkopfzeilen, die den Netzwerkpfad angeben, den eine Nachricht vom Absender zum Empfänger nimmt. Er kann auch benutzerdefinierte Nachrichtenkopfzeilen umfassen, die App-Daten für die Nachricht enthalten. <br><br> Wird nur bei Anwenden einer `$select`-Abfrageoption zurückgegeben. Schreibgeschützt.|
|internetMessageId | Zeichenfolge | Die Nachrichten-ID im von [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) angegebenen Format. Kann nur aktualisiert werden, wenn **isDraft** „true“ ist.|
|isDeliveryReceiptRequested|Boolean|Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.|
|isDraft|Boolean|Gibt an, ob die Nachricht ein Entwurf ist. Eine Nachricht ist ein Entwurf, solange sie noch nicht gesendet wurde.|
|isRead|Boolean|Gibt an, ob die Nachricht gelesen wurde.|
|isReadReceiptRequested|Boolean|Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.|
|lastModifiedDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht zuletzt geändert wurde.|
|mentionsPreview|[mentionsPreview](mentionspreview.md)|Informationen zu Erwähnungen in der Nachricht. Bei der Verarbeitung einer `GET` /messages-Anforderung legt der Server diese Eigenschaft fest und fügt sie standardmäßig in die Antwort ein. Der Server gibt Null zurück, wenn es in der Nachricht keine Erwähnungen gibt. Optional. |
|parentFolderId|String|Der eindeutige Bezeichner für das übergeordnete mailFolder-Element der Nachricht.|
|receivedDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht erhalten wurde.|
|replyTo|[recipient](recipient.md) collection|Die E-Mail-Adressen, die beim Antworten verwendet werden sollen.|
|sender|[Empfänger](recipient.md)|Das Konto, das tatsächlich verwendet wird, um die Nachricht zu generieren. In den meisten Fällen ist dieser Wert identisch mit dem der **from**-Eigenschaft. Sie können diese Eigenschaft auf einen anderen Wert festlegen, wenn Sie eine Nachricht aus einem [freigegebenen Postfach](https://docs.microsoft.com/de-DE/exchange/collaboration/shared-mailboxes/shared-mailboxes) oder als [Stellvertretung](https://support.office.com/de-DE/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926) senden. Der Wert muss auf jeden Fall dem tatsächlich verwendeten Postfach entsprechen. Weitere Informationen über das [Festlegen der Eigenschaften „from“ und „sender“](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) einer Nachricht.|
|sentDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht gesendet wurde.|
|Betreff|String|Der Betreff der Nachricht.|
|toRecipients|[recipient](recipient.md) collection|Die An:-Empfänger der Nachricht.|
|uniqueBody|[itemBody](itembody.md)|Der Teil des Nachrichtentexts, der nur in der aktuellen Nachricht vorhanden ist. **uniqueBody** wird nicht standardmäßig zurückgegeben, kann aber für eine bestimmte Nachricht mithilfe der Abfrage `?$select=uniqueBody` abgerufen werden. Er kann im HTML- oder Textformat vorliegen.|
|unsubscribeData|String|Die gültigen Einträge, die vom List-Unsubscribe-Header analysiert werden.  Dies sind die Daten für den E-Mail-Befehl im List-Unsubscribe-Header, wenn die UnsubscribeeEnabled-Eigenschaft „true“ ist.|
|unsubscribeEnabled|Boolesch|Gibt an, ob die Nachricht zum Kündigen des Abonnements aktiviert ist.  Wenn der list-Unsubscribe-Header „rfc-2369“ entspricht, ist der Wert „true“.|
|webLink|String|Die URL zum Öffnen der Nachricht in Outlook Web App.<br><br>Sie können am Ende der URL das Argument „ispopout“ anhängen, um zu ändern, wie die Nachricht angezeigt wird. Wenn „ispopout“ nicht vorhanden oder auf 1 festgelegt ist, wird die Nachricht in einem Popout-Fenster angezeigt. Wenn „ispopout“ auf 0 festgelegt ist, zeigt der Browser die Nachricht in Outlook Web App im Prüffensterbereich an.<br><br>Die Nachricht wird im Browser geöffnet, wenn Sie über Outlook Web App bei Ihrem Postfach angemeldet sind. Sie werden aufgefordert, sich anzumelden, wenn Sie noch nicht beim Browser angemeldet sind.<br><br>Auf diese URL kann von einem iFrame aus zugegriffen werden.|


## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Anlagen|[Anlagensammlung](attachment.md)|Die [fileAttachment](fileattachment.md)- und [itemAttachment](itemattachment.md)-Anlagen der Nachricht.|
|Erweiterungen|[Erweiterungssammlung](extension.md)| Die Sammlung der für die Nachricht definierten offenen Erweiterungen. Nullwerte zulassend.|
|Erwähnungen|[Erwähnungssammlung](mention.md) | Eine Sammlung von Erwähnungen in der Nachricht, sortiert nach **createdDateTime** vom neuesten zum ältesten Element. Standardmäßig gibt `GET` /message diese Eigenschaft nicht zurück, es sei denn, Sie wenden `$expand` auf die Eigenschaft an.|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung| Die Sammlung der für die Nachricht definierten mehrwertigen erweiterten Eigenschaften. Nullwerte zulassend.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung| Die Sammlung der für die Nachricht definierten einwertigen erweiterten Eigenschaften. Nullwerte zulassend.|

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Nachrichten auflisten](../api/user-list-messages.md) |Sammlung von [Nachrichten](message.md) | Dient zum Abrufen aller Nachrichten im Postfach des angemeldeten Benutzers (einschließlich der Ordner „Gelöschte Elemente“ und „Clutter“). |
|[Nachricht erstellen](../api/user-post-messages.md) | [Nachricht](message.md) | Erstellt einen Entwurf einer neuen Nachricht. |
|[Nachricht abrufen](../api/message-get.md) | [Nachricht](message.md) |Liest Eigenschaften und Beziehungen des Nachrichtenobjekts.|
|[Aktualisieren](../api/message-update.md) | [Nachricht](message.md) |Aktualisiert das Nachrichtenobjekt. |
|[Löschen](../api/message-delete.md) | Keiner |Löscht das Nachrichtenobjekt. |
|[Kopieren](../api/message-copy.md)|[Nachricht](message.md)|Kopiert eine Nachricht in einen Ordner.|
|[createForward](../api/message-createforward.md)|[Nachricht](message.md)|Erstellt einen Entwurf einer Weiterleitungsnachricht, um in einem **createForward**-Aufruf einen Kommentar einzuschließen oder Nachrichteneigenschaften zu aktualisieren. Sie können den Entwurf dann [aktualisieren](../api/message-update.md) oder [senden](../api/message-send.md).|
|[createReply](../api/message-createreply.md)|[Nachricht](message.md)|Erstellt einen Entwurf einer Antwortnachricht, um in einem **createReply**-Aufruf einen Kommentar einzuschließen oder Nachrichteneigenschaften zu aktualisieren. Sie können den Entwurf dann [aktualisieren](../api/message-update.md) oder [senden](../api/message-send.md).|
|[createReplyAll](../api/message-createreplyall.md)|[Nachricht](message.md)|Erstellt einen Entwurf einer Antwortnachricht an alle Empfänger, um in einem **createReplyAll**-Aufruf einen Kommentar einzuschließen oder Nachrichteneigenschaften zu aktualisieren. Sie können den Entwurf dann [aktualisieren](../api/message-update.md) oder [senden](../api/message-send.md).|
|[delta](../api/message-delta.md)|[message](message.md)-Sammlung| Dient zum Abrufen eines Satzes von Nachrichten, die einem bestimmten Ordner hinzugefügt bzw. daraus gelöscht oder darin aktualisiert wurden.|
|[forward](../api/message-forward.md)|Keine|Leitet eine Nachricht weiter, fügt einen Kommentar hinzu oder ändert aktualisierbare Eigenschaften in einem **forward**-Aufruf. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.|
|[move](../api/message-move.md)|[Nachricht](message.md)|Verschiebt eine Nachricht in einen Ordner. Dadurch wird eine neue Kopie der Nachricht im Zielordner erstellt.|
|[Antworten](../api/message-reply.md)|Keine|Antwortet dem Absender einer Nachricht, fügt einen Kommentar hinzu oder ändert aktualisierbare Eigenschaften in einem **reply**-Aufruf. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.|
|[replyAll](../api/message-replyall.md)|Keine|Antwortet allen Empfänger einer Nachricht, indem durch Verwendung der **replyAll**-Methode ein Kommentar angegeben und alle aktualisierbaren Eigenschaften für die Antwort geändert werden. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.|
|[send](../api/message-send.md)|Keine|Sendet einen zuvor erstellten Nachrichtenentwurf. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.|
|[unsubscribe](../api/message-unsubscribe.md)|Keine|Sendet eine Nachricht unter Verwendung der Daten und der Adresse, die im ersten mailto-Befehl im List-Unsubscribe-Header angegeben wurden.|
|**Anlagen**| | |
|[Anlagen auflisten](../api/message-list-attachments.md) |[attachment](attachment.md)-Sammlung| Ruft alle Anlagen einer Nachricht ab.|
|[Anlage hinzufügen](../api/message-post-attachments.md) |[Anlage](attachment.md)| Fügt einer Nachricht eine neue Anlage durch Veröffentlichen in der Anlagensammlung hinzu.|
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften zu einer neuen oder vorhandenen Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Dient zum Abrufen einer offenen Erweiterung, die durch den Erweiterungsnamen identifiziert wird.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](/graph/extensibility-schema-groups) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|
|**Erweiterte Eigenschaften**| | |
|[Einwertige erweiterte Eigenschaft erstellen](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[Nachricht](message.md)  |Erstellt eine oder mehrere einwertige erweiterte Eigenschaften in einer neuen oder vorhandenen Nachricht.   |
|[Nachricht mit einwertiger erweiterter Eigenschaft abrufen](../api/singlevaluelegacyextendedproperty-get.md)  | [Nachricht](message.md) | Ruft mithilfe von `$expand` oder `$filter` Nachrichten mit einer einwertigen erweiterten Eigenschaft ab. |
|[Mehrwertige erweiterte Eigenschaft erstellen](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [Nachricht](message.md) | Erstellt eine oder mehrere mehrwertige erweiterte Eigenschaften in einer neuen oder vorhandenen Nachricht.  |
|[Nachricht mit mehrwertiger erweiterter Eigenschaft abrufen](../api/multivaluelegacyextendedproperty-get.md)  | [Nachricht](message.md) | Ruft eine Nachricht mit einer mehrwertigen erweiterten Eigenschaft mithilfe von `$expand` ab. |

## <a name="see-also"></a>Siehe auch

- [Postfacheinstellungen abrufen](../api/user-get-mailboxsettings.md) 
- [Postfacheinstellungen aktualisieren](../api/user-update-mailboxsettings.md)
- [Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten](/graph/delta-query-overview)
- [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](/graph/delta-query-messages)
- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](/graph/extensibility-open-users)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/message.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}

