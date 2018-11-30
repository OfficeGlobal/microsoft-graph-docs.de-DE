---
title: Ressourcentyp deviceAndAppManagementAssignedRoleIds
description: Noch nicht dokumentiert
ms.openlocfilehash: 9d9fbf9bc6dcfa422316a236dfd890369d069c2f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062474"
---
# <a name="deviceandappmanagementassignedroleids-resource-type"></a>Ressourcentyp deviceAndAppManagementAssignedRoleIds

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|roleDefinitionIds|GUID-Sammlung|Role-Definition-IDs für die spezifische Rollendefinitionen, die einem Benutzer zugewiesen.|
|roleAssignmentIds|GUID-Sammlung|Role Assignment-IDs für die spezifische Rollenzuweisungen, die einem Benutzer zugewiesen.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleIds"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignedRoleIds",
  "roleDefinitionIds": [
    "Guid"
  ],
  "roleAssignmentIds": [
    "Guid"
  ]
}
```





