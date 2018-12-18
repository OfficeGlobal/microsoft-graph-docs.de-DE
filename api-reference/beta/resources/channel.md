---
title: DDE-Kanal Ressourcentyp
description: 'Ein Kanal ist eine Auflistung von ChatMessages innerhalb eines Teams. '
author: nkramer
ms.openlocfilehash: 18a3293b757e641eab98b166a43ce023762ccc6d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326775"
---
# <a name="channel-resource-type"></a>DDE-Kanal Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ein Kanal ist eine Auflistung von [ChatMessages](chatmessage.md) in einem [Team](../resources/team.md). Ein Kanal stellt ein Thema und daher eine logische Isolierung von Diskussion, innerhalb eines Teams. Beispiele für können DDE-Kanal "Freitag Team Mittagessen" und "Diskussion über Architektur" Channel sein.


## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Liste Kanäle](../api/channel-list.md) | [Kanal](channel.md) -Auflistung | Rufen Sie die Liste der Kanäle in dieser Gruppe.|
|[Erstellen von DDE-Kanal](../api/channel-post.md) | [DDE-Kanal](channel.md) | Erstellen Sie einen neuen Kanal durch das Einbeziehen von den Anzeigenamen und die Beschreibung ein.|
|[Abrufen von DDE-Kanal](../api/channel-get.md) | [DDE-Kanal](channel.md) | Lesen Sie Eigenschaften und Beziehungen des Kanals.|
|[Aktualisieren der DDE-Kanal](../api/channel-patch.md) | [DDE-Kanal](channel.md) | Aktualisieren Sie die Eigenschaften des Kanals.|
|[DDE-Kanal löschen](../api/channel-delete.md) | Keines | Löschen Sie einen Kanal.|
|[Liste Channel Nachrichten](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Abrufen von Nachrichten in einem Kanal |
|[Chat Thread erstellen](../api/channel-post-chatthreads.md) | [ChatThread](chatthread.md) -Auflistung| Erstellen Sie einen Chat Thread in den angegebenen DDE-Kanal.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|description|String|Optionale Beschreibung für den Kanal.|
|displayName|String|Channel-Namen, die dem Benutzer in Microsoft-Teams, erscheint.|
|id|String|Eindeutiger Bezeichner der Kanäle. Schreibgeschützt.|
|isFavoriteByDefault|Boolesch|Gibt an, ob der Kanal automatisch "Favoriten" für alle Mitglieder des Teams gekennzeichnet werden soll. Standard: `false`.|
|E-Mail|Boolesch| Die e-Mail-Adresse zum Senden von Nachrichten an den Kanal. Schreibgeschützt.|
|webUrl|String|Ein Hyperlink, zu dem navigiert an den Kanal in Microsoft-Teams. Dies ist die URL, die Sie erhalten, wenn Sie mit der rechten Maustaste in eines Kanals in Microsoft-Teams, und wählen Sie Get-Link Kanal aus. Diese URL sollte als nicht transparentes Blob behandelt und nicht analysiert werden. Schreibgeschützt.|


## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Nachrichten|[ChatMessage](chatmessage.md) -Auflistung|Eine Auflistung aller Nachrichten im Kanal. Eine Navigationseigenschaft. Lässt Nullwerte zu. Diese API wird derzeit nur Lesevorgänge unterstützt, aber der Verfassen von Nachrichten schließlich zu unterstützen.|
|chatThreads|[ChatThread](chatthread.md) -Auflistung|(Dies ist wird phased durch die Eigenschaft Nachrichten) ChatThreads Erstellen neuer Nachrichten aber nicht lesen von Nachrichten unterstützt. ChatThreads ist eine Navigationseigenschaft und zulässig sind.|
|Registerkarten|[TeamsTab](../resources/teamstab.md) -Auflistung|Eine Auflistung aller Registerkarten im Kanal. Eine Navigationseigenschaft.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
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
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
