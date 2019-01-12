---
title: Ressourcentyp conversation
description: Eine Unterhaltung ist eine Sammlung von Threads, und ein Thread enthält Beiträge zu diesem Thread. Alle Threads und Beiträge in einer Unterhaltung haben denselben Betreff.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5cacad2b9539c398251ffd07899df7beb3c2f378
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991440"
---
# <a name="conversation-resource-type"></a>Ressourcentyp conversation

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Eine Unterhaltung ist eine Sammlung von [Threads](conversationthread.md), und ein Thread enthält Beiträge zu diesem Thread. Alle Threads und Beiträge in einer Unterhaltung haben denselben Betreff.

Diese Ressource unterstützt Abonnieren von [Benachrichtigungen ändern](/graph/webhooks).

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Unterhaltungen auflisten](../api/group-list-conversations.md) | [conversation](conversation.md)-Sammlung |Dient zum Abrufen der Liste von Unterhaltungen in dieser Gruppe.|
|[Erstellen](../api/group-post-conversations.md) |[Unterhaltung](conversation.md)| Erstellen Sie eine neue Unterhaltung, indem Sie einen Thread und einen Beitrag einschließen.|
|[Unterhaltung abrufen](../api/conversation-get.md) | [Unterhaltung](conversation.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des Unterhaltungsobjekts.|
|[Löschen](../api/conversation-delete.md) | Keine |Unterhaltungsobjekt löschen. |
|[Unterhaltungsthreads auflisten](../api/conversation-list-threads.md) |[conversationThread](conversationthread.md)-Sammlung| Dient zum Abrufen aller Threads in einer Gruppenunterhaltung.|
|[Unterhaltungsthread erstellen](../api/conversation-post-threads.md) |[conversationThread](conversationthread.md)-Sammlung| Dient zum Erstellen eines Threads in einer bestimmten Unterhaltung.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|hasAttachments|Boolean|Gibt an, ob einer der Beiträge innerhalb dieser Unterhaltung über mindestens eine Anlage verfügt.|
|id|Zeichenfolge|Die eindeutigen Bezeichner der Unterhaltungen. Schreibgeschützt.|
|lastDeliveredDateTime|DateTimeOffset|Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|Vorschau|Zeichenfolge|Eine kurze Zusammenfassung aus dem Text des neuesten Beitrags in dieser Unterhaltung.|
|Thema|Zeichenfolge|Das Thema der Unterhaltung. Diese Eigenschaft kann festgelegt werden, wenn die Unterhaltung erstellt wird, sie kann jedoch nicht aktualisiert werden.|
|uniqueSenders|Zeichenfolgenauflistung|Alle Benutzer, die eine Nachricht an diese Unterhaltung gesendet haben.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Threads|[conversationThread](conversationthread.md)-Sammlung|Eine Auflistung aller Unterhaltungsthreads in der Unterhaltung. Eine Navigationseigenschaft. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversation"
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
