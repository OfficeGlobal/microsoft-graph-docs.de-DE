---
title: targetedManagedAppPolicyAssignment-Ressourcentyp
description: Der Typ der Bereitstellung von Gruppen oder Apps
author: tfitzmac
ms.openlocfilehash: 89caa9b24f9b22bd064931763fef2361102a689e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303115"
---
# <a name="targetedmanagedapppolicyassignment-resource-type"></a>targetedManagedAppPolicyAssignment-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Der Typ der Bereitstellung von Gruppen oder Apps
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[targetedManagedAppPolicyAssignments auflisten](../api/intune-mam-targetedmanagedapppolicyassignment-list.md)|[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)-Objekte.|
|[targetedManagedAppPolicyAssignment abrufen](../api/intune-mam-targetedmanagedapppolicyassignment-get.md)|[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|Lesen von Eigenschaften und Beziehungen des [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)-Objekts.|
|[targetedManagedAppPolicyAssignment löschen](../api/intune-mam-targetedmanagedapppolicyassignment-delete.md)|Keine|Löscht ein [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)-Objekt.|
|[targetedManagedAppPolicyAssignment aktualisieren](../api/intune-mam-targetedmanagedapppolicyassignment-update.md)|[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|Aktualisieren der Eigenschaften eines [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Id|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Bezeichner für die Bereitstellung einer Gruppe oder App|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppPolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



