---
title: channel-Ressourcentyp
description: 'Ein Kanal ist eine Auflistung von Nachrichten innerhalb eines Teams. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 2bebf78e4ad31047289bff77e681c34d92a94abf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163714"
---
# <a name="channel-resource-type"></a>channel-Ressourcentyp



Ein Kanal ist eine Auflistung von Nachrichten innerhalb eines [Teams](../resources/team.md). Ein Kanal stellt ein Thema und somit eine logische Trennung einer Unterhaltung in einem Team dar. Beispiele sind der Kanal „Mittagessen mit dem Team am Freitag“ und „Besprechung der Architektur“.


## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[List channels](../api/channel-list.md) | [channel](channel.md)-Auflistung | Abrufen der Liste von Kanälen in diesem Team.|
|[Create channel](../api/channel-post.md) | [channel](channel.md) | Erstellen eines neuen Kanals durch Einschließen des Anzeigenamen und der Beschreibung.|
|[Get channel](../api/channel-get.md) | [channel](channel.md) | Lesen von Eigenschaften und Beziehungen des Kanals.|
|[Updatekanal](../api/channel-patch.md) | [channel](channel.md) | Aktualisieren der Eigenschaften des Kanals.|
|[Delete channel](../api/channel-delete.md) | Keine | Löschen eines Kanals.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|description|Zeichenfolge|Optionale Textbeschreibung für den Kanal.|
|displayName|Zeichenfolge|Kanalname wie er in Microsoft Teams für den Benutzer angezeigt wird.|
|id|Zeichenfolge|Eindeutiger Bezeichner für den Kanal. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Registerkarten|[teamsTab](../resources/teamstab.md)-Auflistung|Eine Auflistung aller Registerkarten im Kanal. Eine Navigationseigenschaft.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)"
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
