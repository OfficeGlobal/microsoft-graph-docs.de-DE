---
title: Ressourcentyp audioConferencing
description: Stellt Access Telefoninformationen für einen OnlineMeeting.
ms.openlocfilehash: dd23c6ade282e081482a8c079491644c663b4054
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060468"
---
# <a name="audioconferencing-resource-type"></a>Ressourcentyp audioConferencing

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt Access Telefoninformationen für einen [OnlineMeeting](onlinemeeting.md).

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ    | Beschreibung                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| dialinUrl           | String  | Eine URL, die extern zugängliche Webseite, die Einwahlinformationen enthält. |
| leaderPasscode      | String  | Der Leiter Kennwort zum Verbinden mit dem Audio Conference Provider erforderlich.      |
| participantPasscode | String  | Die Teilnehmer das Kennwort zum Verbinden mit dem Audio Conference Provider erforderlich. |
| tollFreeNumber      | String  | Die gebührenfreie Telefonnummer für die Audio Conference Provider die Verbindung.              |
| tollNumber          | String  | Die gebührenpflichtige Telefonnummer für die Audio Conference Provider die Verbindung.                   |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "leaderPasscode": "String",
  "participantPasscode": "String",
  "tollFreeNumber": "String",
  "tollNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
