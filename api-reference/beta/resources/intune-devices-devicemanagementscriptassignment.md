---
title: Ressourcentyp deviceManagementScriptAssignment
description: Enthält Eigenschaften, die zum Zuweisen eines Verwaltungsskripts Gerät zu einer Gruppe.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d335f31ceed7ca670981e7702b69950b7f5a864a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923894"
---
# <a name="devicemanagementscriptassignment-resource-type"></a>Ressourcentyp deviceManagementScriptAssignment

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften, die zum Zuweisen eines Verwaltungsskripts Gerät zu einer Gruppe.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste deviceManagementScriptAssignments](../api/intune-devices-devicemanagementscriptassignment-list.md)|[DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Auflistung|Listeneigenschaften und Beziehungen der [DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Objekte.|
|[Abrufen von deviceManagementScriptAssignment](../api/intune-devices-devicemanagementscriptassignment-get.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|Lesen Sie Eigenschaften und Beziehungen des [DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Objekts.|
|[Erstellen von deviceManagementScriptAssignment](../api/intune-devices-devicemanagementscriptassignment-create.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|Erstellen eines neuen [DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Objekts.|
|[DeviceManagementScriptAssignment löschen](../api/intune-devices-devicemanagementscriptassignment-delete.md)|Keine|Löscht eine [DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).|
|[DeviceManagementScriptAssignment aktualisieren](../api/intune-devices-devicemanagementscriptassignment-update.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|Aktualisieren Sie die Eigenschaften eines [DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Taste der Gerät Management Skript Gruppe Zuordnung Entität.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Die Id des Azure Active Directory-Gruppe verwenden wir das Skript Inhaltsadressierung für.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





