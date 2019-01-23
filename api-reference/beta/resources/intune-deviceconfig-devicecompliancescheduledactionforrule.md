---
title: deviceComplianceScheduledActionForRule-Ressourcentyp
description: Geplante Aktion für eine Regel
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a2cb485b83ce11c3f3dcca51d11d9a0cfb977195
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425302"
---
# <a name="devicecompliancescheduledactionforrule-resource-type"></a>deviceComplianceScheduledActionForRule-Ressourcentyp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Geplante Aktion für eine Regel

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceComplianceScheduledActionForRules auflisten](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-list.md)|[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection|Auflisten von Eigenschaften und Beziehungen der [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)-Objekte.|
|[deviceComplianceScheduledActionForRule abrufen](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-get.md)|[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|Lesen von Eigenschaften und Beziehungen des [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)-Objekts.|
|[deviceComplianceScheduledActionForRule erstellen](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-create.md)|[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|Erstellen eines neuen [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)-Objekts.|
|[deviceComplianceScheduledActionForRule löschen](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-delete.md)|Keine|Löscht ein [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)-Objekt.|
|[deviceComplianceScheduledActionForRule aktualisieren](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-update.md)|[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|Aktualisieren der Eigenschaften eines [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|ruleName|String|Name der Regel, für die diese geplante Aktion gilt.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|scheduledActionConfigurations|[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Sammlung|Die Liste der geplanten Aktionskonfigurationen für diese Compliance-Richtlinie.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScheduledActionForRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "String (identifier)",
  "ruleName": "String"
}
```




