---
title: channel-Ressourcentyp
description: 'Ein Kanal ist eine Auflistung von chatMessages innerhalb eines Teams. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: d58a3e0b867a675e378fa126108331fd5b27856c
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29994468"
---
# <a name="channel-resource-type"></a>channel-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein Kanal ist eine Auflistung von [chatMessages](chatmessage.md) innerhalb eines [Teams](../resources/team.md). Ein Kanal stellt ein Thema und somit eine logische Trennung einer Unterhaltung in einem Team dar. Beispiele sind der Kanal „Mittagessen mit dem Team am Freitag“ und „Besprechung der Architektur“.


## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[List channels](../api/channel-list.md) | [channel](channel.md)-Auflistung | Abrufen der Liste von Kanälen in diesem Team.|
|[Create channel](../api/channel-post.md) | [channel](channel.md) | Erstellen eines neuen Kanals durch Einschließen des Anzeigenamen und der Beschreibung.|
|[Get channel](../api/channel-get.md) | [channel](channel.md) | Lesen von Eigenschaften und Beziehungen des Kanals.|
|[Updatekanal](../api/channel-patch.md) | [channel](channel.md) | Aktualisieren der Eigenschaften des Kanals.|
|[Delete channel](../api/channel-delete.md) | Keine | Löschen eines Kanals.|
|[List channel messages](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Abrufen von Nachrichten in einem Kanal. |
|[Kanalnachricht senden](../api/channel-post-chatmessage.md)  | [chatMessage](../resources/chatmessage.md) | [Senden einer Nachricht an einen Kanal](../api/channel-post-chatmessage.md) |


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|description|Zeichenfolge|Optionale Textbeschreibung für den Kanal.|
|displayName|Zeichenfolge|Kanalname wie er in Microsoft Teams für den Benutzer angezeigt wird.|
|id|Zeichenfolge|Eindeutiger Bezeichner für den Kanal. Schreibgeschützt.|
|isFavoriteByDefault|Boolescher Wert|Gibt an, ob der Kanal automatisch für alle Mitglieder des Teams als „Favorit“ gekennzeichnet werden soll. Standard: `false`.|
|email|Boolescher Wert| Die E-Mail-Adresse zum Senden von Nachrichten an den Kanal. Schreibgeschützt.|
|webUrl|Zeichenfolge|Ein Link, der in Microsoft Teams zum Kanal navigiert. Dies ist die URL, die Sie erhalten, wenn Sie mit der rechten Maustaste in Microsoft Teams auf einen Kanal klicken, und auf die Option zum Abrufen des Links zum Kanal klicken. Diese URL sollte als nicht transparenter Blob behandelt und nicht analysiert werden. Schreibgeschützt.|


## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|messages|[chatMessage](chatmessage.md)-Auflistung|Eine Auflistung aller Nachrichten im Kanal. Eine Navigationseigenschaft. Nullwerte zulassend. Diese API unterstützt derzeit nur das Lesen von Nachrichten, das Schreiben wird aber auch bald unterstützt.|
|Registerkarten|[teamsTab](../resources/teamstab.md)-Auflistung|Eine Auflistung aller Registerkarten im Kanal. Eine Navigationseigenschaft.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messages"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/channel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
