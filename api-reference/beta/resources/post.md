---
title: Beitragsressourcentyp
description: Stellt ein einzelnes Post-Element innerhalb einer ConverstaionThread Entität.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 554892bdfed45d0fba9b90a084db67c0bb329486
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519955"
---
# <a name="post-resource-type"></a>Beitragsressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt ein einzelnes Post-Element innerhalb einer [ConverstaionThread](conversationthread.md) Entität.

Zwar können Sie Beiträge nicht explizit erstellen; es wird jedoch bei jedem der folgenden Vorgänge ein Beitrag erstellt:

* [auf einen vorhandenen Beitrag antworten](../api/post-reply.md) 
* [auf einen vorhandenen Thread antworten](../api/conversationthread-reply.md) 
* [einen Thread in einer neuen Unterhaltung erstellen](../api/group-post-threads.md)
* [eine neue Unterhaltung erstellen](../api/group-post-conversations.md)

Diese Ressource ermöglicht es Ihnen, benutzerdefinierten Eigenschaften mithilfe von [Erweiterungen](/graph/extensibility-overview) eigene Daten hinzuzufügen.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "extensions",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.post"
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
  "importance": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "newParticipants": [{"@odata.type": "microsoft.graph.recipient"}],
  "receivedDateTime": "String (timestamp)",
  "sender": {"@odata.type": "microsoft.graph.recipient"}
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|body|[itemBody](itembody.md)|Der Inhalt des Beitrags. Dies ist eine Standardeigenschaft. Für diese Eigenschaft sind Nullwerte zulässig.|
|categories|Zeichenfolgenauflistung|Die Kategorien, die mit dem Beitrag verknüpft sind. Jeder Kategorie entspricht die **DisplayName** -Eigenschaft des ein [OutlookCategory](outlookcategory.md) , der für einen Benutzer definiert wurde.|
|changeKey|String|Gibt die Version des Beitrags an. Jedes Mal, wenn der Beitrag geändert wird, wird auch ChangeKey geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen.|
|conversationId|String|Eindeutige ID der Unterhaltung. Schreibgeschützt.|
|conversationThreadId|String|Eindeutige ID des Unterhaltungsthreads. Schreibgeschützt.|
|createdDateTime|DateTimeOffset|Gibt an, wann der Beitrag erstellt wurde. Der DateTimeOffset-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|Von|[Empfänger](recipient.md)|Wird in Zugriffsszenarien mit Stellvertretungen verwendet. Gibt an, wer die Nachricht im Auftrag eines anderen Benutzers veröffentlicht hat. Dies ist eine Standardeigenschaft.|
|hasAttachments|Boolescher Wert|Gibt an, ob der Beitrag mindestens eine Anlage enthält. Dies ist eine Standardeigenschaft.|
|id|String| Schreibgeschützt|
|importance | Zeichenfolge | Die Bedeutung der einer Gruppe Post: `low`, `normal`, `high`. |
|lastModifiedDateTime|DateTimeOffset|Gibt an, wann der Beitrag zuletzt geändert wurde. Der DateTimeOffset-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|newParticipants|[recipient](recipient.md) collection|Teilnehmer einer Unterhaltung, die im Rahmen des Beitrags zu dem Thread hinzugefügt wurden.|
|receivedDateTime|DateTimeOffset|Gibt an, wann der Beitrag empfangen wurde. Der DateTimeOffset-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|sender|[recipient](recipient.md)|Enthält die E-Mail-Adresse des Absenders. Bei dem Sender-Wert wird davon ausgegangen, dass dies die Adresse des authentifizierten Benutzers ist, wenn Absender nicht angegeben wurde. Dies ist eine Standardeigenschaft.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Anlagen|[attachment](attachment.md)-Sammlung|Die Auflistung von [FileAttachment](fileattachment.md), [ItemAttachment](itemattachment.md)und [ReferenceAttachment](referenceattachment.md) Anlagen für die Bereitstellung. Schreibgeschützt. Nullwerte zulassend.|
|Erweiterungen|[Erweiterungssammlung](extension.md)|Die Sammlung der für den Beitrag definierten offenen Erweiterungen. Schreibgeschützt. Lässt Nullwerte zu.|
|inReplyTo|[Post](post.md)|Frühere Beitrags, den dieser Beitrag in der [ConversationThread](conversationthread.md)beantwortet wird. Schreibgeschützt.|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung| Die Sammlung erweiterter mehrwertiger Eigenschaften, die für den Beitrag definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung| Die Sammlung erweiterter einwertiger Eigenschaften, die für den Beitrag definiert sind. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[List posts](../api/conversationthread-list-posts.md) | [post](post.md) |Dient zum Abrufen der Beiträge des angegebenen Threads. |
|[Get post](../api/post-get.md) | [post](post.md) |Dient zum Abrufen der Eigenschaften und der Beziehungen eines Beitrags in einem angegebenen Thread.|
|[Reply](../api/post-reply.md)|Keine|Dient zum Antworten auf einen Beitrag und zum Hinzufügen eines neuen Beitrags zum angegebenen Thread in einer Gruppenunterhaltung.|
|[Forward](../api/post-forward.md)|Keine|Dient zum Weiterleiten eines Beitrags an einen Empfänger.|
|**Anlagen**| | |
|[Anlagen auflisten](../api/post-list-attachments.md) |[attachment](attachment.md) collection| Ruft alle Anlagen für einen Beitrag ab.|
|[Hinzufügen von Anlagen](../api/post-post-attachments.md) |[attachment](attachment.md)| Dient zum Hinzufügen einer Anlage zu einem Beitrag. |
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften zu einer neuen oder vorhandenen Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Dient zum Abrufen einer offenen Erweiterung, die durch den Erweiterungsnamen identifiziert wird.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](/graph/extensibility-schema-groups) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|
|**Erweiterte Eigenschaften**| | |
|[Einwertige erweiterte Eigenschaft erstellen](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[post](post.md)  |Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen Beitrag.   |
|[Get post with single-value extended property](../api/singlevaluelegacyextendedproperty-get.md)  | [post](post.md) | Dient zum Abrufen von Beiträgen mit einer erweiterten einwertigen Eigenschaft mithilfe von `$expand` oder `$filter`. |
|[Create multi-value extended property](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [post](post.md) | Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen Beitrag  |
|[Get post with multi-value extended property](../api/multivaluelegacyextendedproperty-get.md)  | [post](post.md) | Dient zum Abrufen eines Beitrags mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`. |

## <a name="see-also"></a>Siehe auch

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](/graph/extensibility-open-users)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
