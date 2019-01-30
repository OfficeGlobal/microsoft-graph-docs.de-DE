---
title: " Ressourcentyp secureScoreControlStateUpdate"
description: Diese Ressource enthält Verlauf von Zustände des Steuerelements durch Benutzer aktualisiert (Steuerelementzustände gehören Standard, ignoriert, ThirdParty, überprüft).
localization_priority: Normal
ms.openlocfilehash: 8d8c3122a6263ebc7b10b5edfb823953e2d587fc
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641729"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>Ressourcentyp secureScoreControlStateUpdate
Enthält den Verlauf der vom Benutzer aktualisiert Steuerelementzustände (Steuerelementzustände gehören Standard, ignoriert, ThirdParty, überprüft).

|Eigenschaft |Typ |Beschreibung |
|:--|:--|:--|
|assignedTo | string | Weisen Sie das Steuerelement dem Benutzer, die die Aktion |
|Kommentar | string | Enthält Informationen zum Steuerelement optionalen Kommentar |
|state | string | Zustand des Steuerelements mit PATCH-Befehl geändert werden kann (Ex: ignoriert, ThirdParty usw.) |
|updatedBy | string |ID des Benutzers, der Mandant Status aktualisiert |
|updatedDateTime | DateTimeOffset? |Uhrzeit, an welches Steuerelement Zustand aktualisiert wurde |
 ## <a name="json-representation"></a>JSON-Darstellung
 Es folgt eine JSON-Darstellung der Ressource.
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "Double",
  "state": "Double",
  "updatedBy": "Double",
  "updatedDateTime": "Double"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
