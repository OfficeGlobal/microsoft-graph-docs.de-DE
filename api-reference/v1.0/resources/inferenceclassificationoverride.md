---
title: inferenceClassificationOverride-Ressourcentyp
description: Stellt die Außerkraftsetzung eines Benutzers dafür dar, wie eingehende Nachrichten von einem bestimmten Absender immer klassifiziert werden sollen.
localization_priority: Normal
ms.openlocfilehash: 8df0f1e5fa34c630c51de7c73234e6092448f867
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885064"
---
# <a name="inferenceclassificationoverride-resource-type"></a>inferenceClassificationOverride-Ressourcentyp

Stellt die Außerkraftsetzung eines Benutzers dafür dar, wie eingehende Nachrichten von einem bestimmten Absender immer klassifiziert werden sollen.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Update](../api/inferenceclassificationoverride-update.md) | [inferenceClassificationOverride](inferenceclassificationoverride.md) |Ändern Sie das **ClassifyAs** -Feld einer Außerkraftsetzung wie angegeben. |
|[Delete](../api/inferenceclassificationoverride-delete.md) | Keine |Löscht eine Außerkraftsetzung, die durch ihre ID angegeben ist. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|classifyAs|inferenceClassificationType| Gibt an, wie eingehende-Nachrichten von einer bestimmten Absender sollte stets als klassifiziert werden. Die möglichen Werte sind: `focused`, `other`.|
|id|string| Der eindeutige Bezeichner der Außerkraftsetzung. Schreibgeschützt.|
|senderEmailAddress|[emailAddress](emailaddress.md)|Die E-Mail-Adressinformationen des Absenders, für den die Außerkraftsetzung erstellt wird.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}-->

```json
{
  "classifyAs": "string",
  "id": "string (identifier)",
  "senderEmailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
