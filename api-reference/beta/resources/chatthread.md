---
title: Ressourcentyp chatThread
description: Eine ChatThread ist eine Auflistung von ChatMessages in Microsoft-Teams.
ms.openlocfilehash: ef8f118ae4354a5e4197802708aecfa1fb6f8cb8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064966"
---
# <a name="chatthread-resource-type"></a>Ressourcentyp chatThread

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Eine ChatThread ist eine Auflistung von [ChatMessages](chatmessage.md) in Microsoft-Teams.

> Derzeit können ChatThreads [in Kanäle erstellt](../api/channel-post-chatthreads.md)werden.  Die Zukunft API Versionen wird beim Lesen der vorhandenen ChatThreads als auch Lesen/Schreiben von direkten Chats zwischen Benutzern, die sich des Bereichs einer Teamwebsite oder einer DDE-Kanal außerhalb unterstützt.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Thread erstellen](../api/channel-post-chatthreads.md) | [chatThread](chatthread.md) |Starten Sie einen neuen Thread in der angegebenen DDE-Kanal, die erste Nachricht bereitstellen.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|rootMessage|[chatMessage](chatmessage.md)| Lässt Nullwerte zu.|
|chatMessages|[ChatMessage](chatmessage.md) -Auflistung| Lässt Nullwerte zu.|

> Auf diese Beziehungen vorhanden sind implizit, kann nicht aber gelesen oder geschrieben.  Zukünftige Betaversionen API unterstützt.

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
  "id": "string (identifier)",
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
