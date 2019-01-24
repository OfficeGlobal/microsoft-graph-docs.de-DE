---
title: chatThread-Ressourcentyp
description: Ein chatThread ist eine Sammlung von chatMessages in Microsoft Teams.
localization_priority: Priority
ms.openlocfilehash: 19365109c2008d52d3597b3d23fc1baefa5cfd1c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399605"
---
# <a name="chatthread-resource-type"></a>chatThread-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
<!-- {
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
