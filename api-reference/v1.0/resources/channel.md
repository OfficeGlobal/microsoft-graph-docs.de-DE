---
title: DDE-Kanal Ressourcentyp
description: 'Ein Kanal ist eine Auflistung von Nachrichten in einem Team. '
ms.openlocfilehash: 17a2e2edb86bfe7e107e69414a70dbe92fe4d3bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017420"
---
# <a name="channel-resource-type"></a>DDE-Kanal Ressourcentyp



Ein Kanal ist eine Auflistung von Nachrichten in einem [Team](../resources/team.md). Ein Kanal stellt ein Thema und daher eine logische Isolierung von Diskussion, innerhalb eines Teams. Beispiele für können DDE-Kanal "Freitag Team Mittagessen" und "Diskussion über Architektur" Channel sein.


## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Liste Kanäle](../api/channel-list.md) | [Kanal](channel.md) -Auflistung | Rufen Sie die Liste der Kanäle in dieser Gruppe.|
|[Erstellen von DDE-Kanal](../api/channel-post.md) | [DDE-Kanal](channel.md) | Erstellen Sie einen neuen Kanal durch das Einbeziehen von den Anzeigenamen und die Beschreibung ein.|
|[Abrufen von DDE-Kanal](../api/channel-get.md) | [DDE-Kanal](channel.md) | Lesen Sie Eigenschaften und Beziehungen des Kanals.|
|[Aktualisieren der DDE-Kanal](../api/channel-patch.md) | [DDE-Kanal](channel.md) | Aktualisieren Sie die Eigenschaften des Kanals.|
|[DDE-Kanal löschen](../api/channel-delete.md) | Keines | Löschen Sie einen Kanal.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|description|String|Optionale Beschreibung für den Kanal.|
|displayName|String|Channel-Namen, die dem Benutzer in Microsoft-Teams, erscheint.|
|id|String|Eindeutiger Bezeichner der Kanäle. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
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
