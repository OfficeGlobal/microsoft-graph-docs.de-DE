---
title: Ressourcentyp audioConferencing
description: Stellt Access Telefoninformationen für einen OnlineMeeting.
author: VinodRavichandran
ms.openlocfilehash: 4e2ee26e6f9a86d50efcb21cd95b84b207488ef1
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380226"
---
# <a name="audioconferencing-resource-type"></a>Ressourcentyp audioConferencing

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt Access Telefoninformationen für einen [OnlineMeeting](onlinemeeting.md).

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ    | Beschreibung                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| dialinUrl           | Zeichenfolge  | Eine URL, die extern zugängliche Webseite, die Einwahlinformationen enthält. |
| leaderPasscode      | Zeichenfolge  | Der Leiter Kennwort zum Verbinden mit dem Audio Conference Provider erforderlich.      |
| participantPasscode | Zeichenfolge  | Die Teilnehmer das Kennwort zum Verbinden mit dem Audio Conference Provider erforderlich. |
| tollFreeNumber      | Zeichenfolge  | Die gebührenfreie Telefonnummer für die Audio Conference Provider die Verbindung.              |
| tollNumber          | Zeichenfolge  | Die gebührenpflichtige Telefonnummer für die Audio Conference Provider die Verbindung.                   |

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
