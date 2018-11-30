---
title: mailFolder-Ressoucentyp
description: Ein mailFolder-Element im Postfach eines Benutzers, wie z. B. Posteingang und Entwürfe. Mailordner können Nachrichten, andere Outlook-Elemente und untergeordnete E-Mail-Ordner enthalten.
ms.openlocfilehash: 96e2b6cf2af9ffbe6a6c66d41efe174d1706074d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017388"
---
# <a name="mailfolder-resource-type"></a>mailFolder-Ressoucentyp

Ein mailFolder-Element im Postfach eines Benutzers, wie z. B. Posteingang und Entwürfe. Mailordner können Nachrichten, andere Outlook-Elemente und untergeordnete E-Mail-Ordner enthalten.

Diese Ressource unterstützt die Verwendung einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen einer [delta](../api/mailfolder-delta.md)-Funktion.

**Bekannte Ordnernamen**

Outlook erstellt standardmäßig bestimmte Ordner für Benutzer. Statt des **ID-** Werts des entsprechenden Ordner für zu diesem Zweck können Sie die bekannte Ordnernamen aus der folgenden Tabelle beim Zugriff auf diese Ordner. Beispielsweise können Sie den Ordner "Entwürfe" unter Verwendung seines bekannte namens mit der folgenden Abfrage abrufen.

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

Bekannte Namen arbeiten unabhängig von dem Gebietsschema des Postfach des Benutzers, der oben genannten Abfrage immer Ordner "Entwürfe" des Benutzers, unabhängig davon, wie heißt zurückgegeben wird.

| Bekannte Ordnername | Beschreibung |
|:-----------------------|:------------|
| Archiv | Bei Verwendung von One_Click Archiv-Features in Outlook-Clients, die dies unterstützen, werden die Nachrichten archivieren Ordner an gesendet. **Hinweis:** Dies ist nicht das gleiche wie das Archivpostfach Feature von Exchange online. |
| Unübersichtlichkeit | Die Unübersichtlichkeit Ordner niedriger Priorität Nachrichten werden in verschoben, beim Verwenden des Features Unübersichtlichkeit. |
| Konflikte | Der Ordner, der miteinander in Konflikt stehende Elemente im Postfach enthält. |
| conversationhistory | Der Ordner, in dem Skype Sofortnachrichtenunterhaltungen speichert (falls Skype dazu konfiguriert ist). |
| deleteditems | Der Ordnerelemente werden in verschoben, wenn sie gelöscht werden. |
| Entwürfe | Der Ordner, der nicht gesendete Nachrichten enthält. |
| Posteingang | Der Posteingangsordner. |
| junkemail | Der junk-e-Mail-Ordner. |
| localfailures | Der Ordner, der Elemente enthält, die auf dem lokalen Client vorhanden, jedoch nicht auf den Server hochgeladen werden konnte. |
| msgfolderroot | Der Ordner "Oberste Ebene des Informationsspeichers". Dieser Ordner ist des übergeordneten Ordners für Ordner, in der normalen e-Mail-Clients, wie beispielsweise dem Posteingang angezeigt werden. |
| Postausgang | Der Ordner Postausgang. |
| recoverableitemsdeletions | Der Ordner, das vorläufig gelöschte Elemente enthält: gelöscht, aus dem Ordner Gelöschte Objekte oder durch Drücken von UMSCHALT + ENTF in Outlook. Dieser Ordner ist nicht sichtbar, alle Outlook-e-Mail-Client, jedoch können Endbenutzer über das Feature **Gelöschte Elemente wiederherstellen, vom Server** in Outlook oder Outlook im Web mit ihm interagieren. |
| Geplant | Der Ordner, der Nachrichten enthält, die im Posteingang mit der Zeitplan in Outlook für iOS eingeblendet geplant werden. |
| SearchFolders | Der übergeordnete Ordner für alle im Postfach des Benutzers definierten Suchordner. |
| Gesendete Elemente | Ordner "Gesendete Elemente". |
| serverfailures | Der Ordner, der Elemente enthält, die auf dem Server vorhanden, aber konnte nicht auf dem lokalen Client synchronisiert werden. |
| syncissues | Der Ordner, der von Outlook erstellten Synchronisierungsprotokolle enthält. |

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:-------|:------------|:------------|
|[Get mailFolder](../api/mailfolder-get.md) | [mailFolder](mailfolder.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des mailFolder-Objekts.|
|[Create MailFolder](../api/mailfolder-post-childfolders.md) |[MailFolder](mailfolder.md)| Dient zum Erstellen eines neuen mailFolder-Elements unter dem aktuellen durch die Veröffentlichung der childFolders-Sammlung.|
|[List childFolders](../api/mailfolder-list-childfolders.md) |[MailFolder](mailfolder.md)-Sammlung| Dient zum Abrufen der Ordnersammlung unter dem angegebenen Ordner. Sie können die `.../me/MailFolders`Verknüpfung zum Abrufen der Ordnersammlung auf oberster Ebene und zum Navigieren zu einem anderen Ordner verwenden.|
|[Create Message](../api/mailfolder-post-messages.md) |[Nachricht](message.md)| Dient zum Erstellen einer neuen Nachricht in dem aktuellen mailFolder-Element durch die Veröffentlichung in der Nachrichtensammlung.|
|[List messages](../api/mailfolder-list-messages.md) |[Nachrichten](message.md)-Sammlung| Dient zum Abrufen aller Nachrichten im Postfach des angemeldeten Benutzers oder Nachrichten in einen bestimmten Ordner im Postfach.|
|[Update](../api/mailfolder-update.md) | [mailFolder](mailfolder.md)|Dient zum Aktualisieren des angegebenen mailFolder-Objekts. |
|[Delete](../api/mailfolder-delete.md) | Keine |Dient zum Löschen des angegebenen mailFolder-Objekts. |
|[copy](../api/mailfolder-copy.md)|[MailFolder](mailfolder.md)|Dient zum Kopieren eines mailFolder-Elements und seiner Inhalte in ein anderes mailFolder-Element.|
|[delta](../api/mailfolder-delta.md)|[mailFolder](mailfolder.md)-Sammlung|Dient zum Abrufen eines Satzes von E-Mail-Ordnern, die dem Postfach des Benutzers hinzugefügt bzw. daraus gelöscht oder entfernt wurden.|
|[move](../api/mailfolder-move.md)|[MailFolder](mailfolder.md)|Dient zum Verschieben eines mailFolder-Elements und seiner Inhalte in ein anderes mailFolder-Element.|
|**Erweiterte Eigenschaften**| | |
|[Create single-value extended property](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[mailFolder](mailfolder.md)  |Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen mailFolder-Element.   |
|[Get mailFolder with single-value extended property](../api/singlevaluelegacyextendedproperty-get.md)  | [mailFolder](mailfolder.md) | Dient zum Abrufen von mailFolders-Elementen mit einer erweiterten einwertigen Eigenschaft mithilfe von `$expand` oder `$filter`. |
|[Create multi-value extended property](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [mailFolder](mailfolder.md) | Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen mailFolder-Element.  |
|[Get mailFolder with multi-value extended property](../api/multivaluelegacyextendedproperty-get.md)  | [mailFolder](mailfolder.md) | Dient zum Abrufen eines mailFolders-Elements mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`. |

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------|:-----|:------------|
|childFolderCount|Int32|Die Anzahl der unmittelbar untergeordneten mailFolders-Elemente in dem aktuellen mailFolder-Element.|
|displayName|String|Der Anzeigename des mailFolder-Elements.|
|id|String|Eindeutiger Bezeichner der MailFolder.|
|parentFolderId|String|Die eindeutige ID für das übergeordnete mailFolder-Element des mailFolder-Elements.|
|totalItemCount|Int32|Anzahl der Elemente im mailFolder-Element.|
|unreadItemCount|Int32|Die Anzahl der Elemente im mailFolder-Element, die als „Ungelesen“ markiert sind.|

**Effizientes Ermitteln der Anzahl von Elementen**

Die `TotalItemCount` und `UnreadItemCount` Eigenschaften eines Ordners können Sie bequem die Anzahl der gelesenen Elemente im Ordner zu berechnen.
Sie können Sie die Abfragen wie folgt zu vermeiden, die erhebliche Wartezeiten auftreten kann:

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

E-Mail-Ordner in Outlook können mehrere Typen von Elementen enthalten, beispielsweise der Posteingang enthalten kann Anforderung Besprechungselemente vom e-Mail-Elemente darstellen. `TotalItemCount`und `UnreadItemCount` Elemente in einem e-Mail-Ordner unabhängig von deren Elementtypen einschließen.

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

- [Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten](/graph/delta-query-overview)
- [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
