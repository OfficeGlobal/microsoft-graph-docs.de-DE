---
title: " Ressourcentyp secureScoreControlStateUpdate"
description: Diese Ressource enthält Verlauf von Zustände des Steuerelements durch Benutzer aktualisiert (Steuerelementzustände gehören Standard, ignoriert, ThirdParty, überprüft).
ms.openlocfilehash: ba98f2fc85f3f8e12355f9acf5d232599a7f29f7
ms.sourcegitcommit: 8feddb85e436be5581557a199f2e46d5b4ebfa21
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/22/2018
ms.locfileid: "27428840"
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
