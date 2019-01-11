---
title: Ressourcentyp audioConferencing
description: Stellt Access Telefoninformationen für einen OnlineMeeting.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 9bd8343f29a797a24044f02aa2a00bd098c35007
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843624"
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
