---
title: " Ressourcentyp secureScoreControlStateUpdate"
description: Diese Ressource enthält Verlauf von Zustände des Steuerelements durch Benutzer aktualisiert (Steuerelementzustände gehören Standard, ignoriert, ThirdParty, überprüft).
localization_priority: Normal
ms.openlocfilehash: 4e626f67579e3dc35fe36f5dcc67b1512c5e7bbc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574390"
---
 ##  <a name="securescorecontrolstateupdate-resource-type"></a>Ressourcentyp secureScoreControlStateUpdate

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Enthält den Verlauf der vom Benutzer aktualisiert Steuerelementzustände (Steuerelementzustände gehören Standard, ignoriert, ThirdParty, überprüft).

|Eigenschaft         | Typ           |Beschreibung                                                  |
|:----------------|:---------------|:------------------------------------------------------------|
| assignedTo      | string         | Weisen Sie das Steuerelement dem Benutzer, die die Aktion     |
| Kommentar         | string         | Enthält Informationen zum Steuerelement optionalen Kommentar                 |
| state           | string         | Zustand des Steuerelements mit PATCH-Befehl geändert werden kann (Ex: ignoriert, ThirdParty usw.) |
| updatedBy       | string         |ID des Benutzers, der Mandant Status aktualisiert                      |
| updatedDateTime | DateTimeOffset |Uhrzeit, an welches Steuerelement Zustand aktualisiert wurde                      |
 

## <a name="json-representation"></a>JSON-Darstellung
 Es folgt eine JSON-Darstellung der Ressource.

 <!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
```json
{
  "assignedTo": "String",
  "comment": "String",
  "state": "String",
  "updatedBy": "String",
  "updatedDateTime": "DateTimeOffset"
}
```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
