---
title: officeClientConfigurationAssignment-Ressourcentyp
description: Office-Client Konfigurations Zuweisung.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e1ca4c32c701271bbb5bf908d20b78538ebc6568
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148153"
---
# <a name="officeclientconfigurationassignment-resource-type"></a>officeClientConfigurationAssignment-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Office-Client Konfigurations Zuweisung.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[OfficeClientConfigurationAssignments aufListen](../api/intune-cirrus-officeclientconfigurationassignment-list.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Objekte.|
|[OfficeClientConfigurationAssignment abrufen](../api/intune-cirrus-officeclientconfigurationassignment-get.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Lesen von Eigenschaften und Beziehungen des [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Objekts.|
|[OfficeClientConfigurationAssignment erstellen](../api/intune-cirrus-officeclientconfigurationassignment-create.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Erstellen eines neuen [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Objekts.|
|[OfficeClientConfigurationAssignment löschen](../api/intune-cirrus-officeclientconfigurationassignment-delete.md)|Keine|Löscht eine [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).|
|[OfficeClientConfigurationAssignment aktualisieren](../api/intune-cirrus-officeclientconfigurationassignment-update.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Aktualisieren der Eigenschaften eines [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|ID des OfficeConfigurationAssignment.|
|target|[officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|Die vom Administrator definierte Zielzuweisung.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```



