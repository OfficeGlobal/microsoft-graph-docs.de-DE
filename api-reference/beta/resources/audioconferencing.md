---
title: Ressourcentyp audioConferencing
description: Stellt Access Telefoninformationen für einen OnlineMeeting.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cd65b094a17ad3fa470471c3ed6dd3908367e578
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977507"
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
