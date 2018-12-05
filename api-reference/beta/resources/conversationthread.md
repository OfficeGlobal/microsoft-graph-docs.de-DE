---
title: Ressourcentyp conversationThread
description: Ein conversationThread ist eine Sammlung von Beiträgen.
ms.openlocfilehash: a63b208e30372c2cced1e440f3a46e605ea26589
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058447"
---
# <a name="conversationthread-resource-type"></a>Ressourcentyp conversationThread

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ein conversationThread ist eine Sammlung von [Beiträgen](post.md).

Die Empfängersammlung des letzten Beitrags besteht aus den aggregierten Empfängern des gesamten Threads. Ein Thread kann eine wachsende Sammlung von Empfängern haben. Ein neuer Thread wird erstellt, wenn ein Empfänger aus dem Thread entfernt wird.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Threads auflisten](../api/group-list-threads.md) | [conversationThread](conversationthread.md)-Sammlung |Ruft alle Threads einer Gruppe ab.|
|[Thread erstellen](../api/group-post-threads.md) | [conversationThread](conversationthread.md) |Beginnt eine neue Unterhaltung, indem zunächst ein Thread erstellt wird. Eine neue Unterhaltung, Unterhaltungsthreads und Beiträge werden in der Gruppe erstellt.|
|[conversationThread abrufen](../api/conversationthread-get.md) | [conversationThread](conversationthread.md) |Dient zum Abrufen eines bestimmten Threads, der zu einer Gruppe gehört. |
|[Aktualisieren](../api/conversationthread-update.md) | [conversationThread](conversationthread.md)  |conversationThread-Objekt aktualisieren. |
|[Löschen](../api/conversationthread-delete.md) | Keine |conversationThread-Objekt löschen. |
|[Antworten](../api/conversationthread-reply.md)|Keine|Antworten Sie auf diesen Thread, indem Sie eine neue Beitragsentität erstellen.|
|[Beiträge auflisten](../api/conversationthread-list-posts.md) |[post](post.md)-Sammlung| Dient zum Abrufen der Beiträge des angegebenen Threads. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Schreibgeschützt.|
|toRecipients|[recipient](recipient.md)-Sammlung|Die An:-Empfänger des Threads.|
|ccRecipients|[recipient](recipient.md)-Sammlung|Die Cc:-Empfänger des Threads.|
|Thema|String|Das Thema der Unterhaltung. Diese Eigenschaft kann festgelegt werden, wenn die Unterhaltung erstellt wird, sie kann jedoch nicht aktualisiert werden.||
|hasAttachments|Boolean|Gibt an, ob einer der Beiträge innerhalb dieses Threads über mindestens eine Anlage verfügt.|
|lastDeliveredDateTime|DateTimeOffset|Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|uniqueSenders|Zeichenfolgenauflistung|Alle Benutzer, die eine Nachricht an diesen Thread gesendet haben.|
|Vorschau|String|Eine kurze Zusammenfassung aus dem Text des neuesten Beitrags in dieser Unterhaltung.|
|isLocked|Boolean|Zeigt an, ob der Thread gesperrt ist.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|posts|[post](post.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversationThread"
}-->

```json
{
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": true,
  "id": "string (identifier)",
  "isLocked": true,
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->