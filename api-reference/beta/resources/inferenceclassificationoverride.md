---
title: inferenceClassificationOverride-Ressourcentyp
description: Stellt sollte Außerkraftsetzung für eingehende von einem bestimmten Absender wie Nachrichten des Benutzers immer als klassifiziert werden
ms.openlocfilehash: 63c753b7af21907717d7d9706d0606726d5670f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059189"
---
# <a name="inferenceclassificationoverride-resource-type"></a>inferenceClassificationOverride-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt einen Benutzer außer Kraft setzen für eingehende wie von einem bestimmten Absender Nachrichten wie in eine [Praxisorientierte Posteingang](manage-focused-inbox.md)immer klassifiziert werden sollen.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Update](../api/inferenceclassificationoverride-update.md) | [inferenceClassificationOverride](inferenceclassificationoverride.md) |Ändern Sie das **ClassifyAs** -Feld einer Außerkraftsetzung wie angegeben. |
|[Delete](../api/inferenceclassificationoverride-delete.md) | Keine |Löscht eine Außerkraftsetzung, die durch ihre ID angegeben ist. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|classifyAs|string| Gibt an, wie eingehende Nachrichten von einem bestimmten Absender immer klassifiziert werden sollen. Mögliche Werte: `focused`, `other`.|
|id|string| Der eindeutige Bezeichner der Außerkraftsetzung. Schreibgeschützt.|
|senderEmailAddress|[emailAddress](emailaddress.md)|Die E-Mail-Adressinformationen des Absenders, für den die Außerkraftsetzung erstellt wird.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
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