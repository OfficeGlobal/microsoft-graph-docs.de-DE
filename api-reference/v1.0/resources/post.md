---
title: Beitragsressourcentyp
description: Stellt ein einzelnes Post-Element in einer conversationThread-Entität dar.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: d594b7f44a39f17427ac395d4cd734d064d8b1ae
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982869"
---
# <a name="post-resource-type"></a>Beitragsressourcentyp
Stellt ein einzelnes Post-Element in einer [conversationThread](conversationthread.md)-Entität dar.

Zwar können Sie Beiträge nicht explizit erstellen; es wird jedoch bei jedem der folgenden Vorgänge ein Beitrag erstellt:

- [auf einen vorhandenen Beitrag antworten](../api/post-reply.md) 
- [auf einen vorhandenen Thread antworten](../api/conversationthread-reply.md) 
- [einen Thread in einer neuen Unterhaltung erstellen](../api/group-post-threads.md)
- [eine neue Unterhaltung erstellen](../api/group-post-conversations.md)

Diese Ressource ermöglicht es Ihnen, benutzerdefinierten Eigenschaften mithilfe von [Erweiterungen](/graph/extensibility-overview) eigene Daten hinzuzufügen.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[List posts](../api/conversationthread-list-posts.md) | [post](post.md) |Dient zum Abrufen der Beiträge des angegebenen Threads. |
|[Get post](../api/post-get.md) | [post](post.md) |Dient zum Abrufen der Eigenschaften und der Beziehungen eines Beitrags in einem angegebenen Thread.|
|[Reply](../api/post-reply.md)|Keine|Dient zum Antworten auf einen Beitrag und zum Hinzufügen eines neuen Beitrags zum angegebenen Thread in einer Gruppenunterhaltung.|
|[Forward](../api/post-forward.md)|Keine|Dient zum Weiterleiten eines Beitrags an einen Empfänger.|
|**Anlagen**| | |
|[List attachments](../api/post-list-attachments.md) |[attachment](attachment.md) collection| Ruft alle Anlagen für einen Beitrag ab.|
|[Hinzufügen von Anlagen](../api/post-post-attachments.md) |[attachment](attachment.md)| Dient zum Hinzufügen einer Anlage zu einem Beitrag. |
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Ruft ein offenes Erweiterungsobjekt oder Objekte basierend auf ihrem Namen oder vollqualifizierten Namen ab.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](/graph/extensibility-schema-groups) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|
|**Erweiterte Eigenschaften**| | |
|[Einwertige erweiterte Eigenschaft erstellen](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[post](post.md)  |Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen Beitrag.   |
|[Get post with single-value extended property](../api/singlevaluelegacyextendedproperty-get.md)  | [post](post.md) | Dient zum Abrufen von Beiträgen mit einer erweiterten einwertigen Eigenschaft mithilfe von `$expand` oder `$filter`. |
|[Create multi-value extended property](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [post](post.md) | Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen Beitrag  |
|[Get post with multi-value extended property](../api/multivaluelegacyextendedproperty-get.md)  | [post](post.md) | Dient zum Abrufen eines Beitrags mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|body|[itemBody](itembody.md)|Der Inhalt des Beitrags. Dies ist eine Standardeigenschaft. Für diese Eigenschaft sind Nullwerte zulässig.|
|categories|Zeichenfolgenauflistung|Die Kategorien, die mit dem Beitrag verknüpft sind.|
|changeKey|Zeichenfolge|Gibt die Version des Beitrags an. Jedes Mal, wenn der Beitrag geändert wird, wird auch ChangeKey geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen.|
|conversationId|Zeichenfolge|Eindeutige ID der Unterhaltung. Schreibgeschützt.|
|conversationThreadId|Zeichenfolge|Eindeutige ID des Unterhaltungsthreads. Schreibgeschützt.|
|createdDateTime|DateTimeOffset|Gibt an, wann der Beitrag erstellt wurde. Der DateTimeOffset-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|Von|[Empfänger](recipient.md)|Wird in Zugriffsszenarien mit Stellvertretungen verwendet. Gibt an, wer die Nachricht im Auftrag eines anderen Benutzers veröffentlicht hat. Dies ist eine Standardeigenschaft.|
|hasAttachments|Boolescher Wert|Gibt an, ob der Beitrag mindestens eine Anlage enthält. Dies ist eine Standardeigenschaft.|
|id|Zeichenfolge| Schreibgeschützt.|
|lastModifiedDateTime|DateTimeOffset|Gibt an, wann der Beitrag zuletzt geändert wurde. Der DateTimeOffset-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|newParticipants|[recipient](recipient.md) collection|Teilnehmer einer Unterhaltung, die im Rahmen des Beitrags zu dem Thread hinzugefügt wurden.|
|receivedDateTime|DateTimeOffset|Gibt an, wann der Beitrag empfangen wurde. Der DateTimeOffset-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|sender|[recipient](recipient.md)|Enthält die E-Mail-Adresse des Absenders. Bei dem Sender-Wert wird davon ausgegangen, dass dies die Adresse des authentifizierten Benutzers ist, wenn Absender nicht angegeben wurde. Dies ist eine Standardeigenschaft.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Anlagen|[Anlagensammlung](attachment.md)| Schreibgeschützt. Lässt Nullwerte zu.|
|Erweiterungen|[Erweiterungssammlung](extension.md)|Die Sammlung der für den Beitrag definierten offenen Erweiterungen. Schreibgeschützt. Lässt Nullwerte zu.|
|inReplyTo|[post](post.md)| Schreibgeschützt.|
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

## <a name="see-also"></a>Weitere Artikel

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](/graph/extensibility-open-users)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
