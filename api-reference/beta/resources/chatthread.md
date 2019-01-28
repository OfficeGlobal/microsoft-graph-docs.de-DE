---
title: chatThread-Ressourcentyp
description: Ein chatThread ist eine Sammlung von chatMessages in Microsoft Teams.
localization_priority: Priority
ms.openlocfilehash: a85b6aea6c48c9295fe88a7412fa7e6b96ee1d3f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521341"
---
# <a name="chatthread-resource-type"></a>chatThread-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein chatThread ist eine Sammlung von [chatMessages](chatmessage.md) in Microsoft Teams.

> Derzeit können chatThreads [in Kanälen erstellt werden](../api/channel-post-chatthreads.md).  In künftigen API-Versionen wird das Lesen von vorhandenen chatThreads sowie das Lesen/Schreiben von direkten Chats zwischen Benutzern, die sich außerhalb des Bereichs eines Teams oder Kanals befinden, unterstützt.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Thread erstellen](../api/channel-post-chatthreads.md) | [chatThread](chatthread.md) |Starten Sie einen neuen Thread in dem angegebenen Kanal, wodurch Sie die erste Nachricht bereitstellen.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|rootMessage|[chatMessage](chatmessage.md)| Nullwerte zulassend.|
|chatMessages|[chatMessage](chatmessage.md)-Sammlung| Nullwerte zulassend.|

> Diese Beziehungen sind derzeit implizit vorhanden, können aber nicht gelesen oder geschrieben werden.  In zukünftigen API-Betaversionen wird dies unterstützt.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatThread"
}-->

```json
{
  "id": "string (identifier)"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatthread.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
