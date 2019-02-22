---
title: windowsManagementApp-Ressourcentyp
description: Entität der Windows-Verwaltungs-app.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a10e3a0779dac787857203941d266d9ab9a7712
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140082"
---
# <a name="windowsmanagementapp-resource-type"></a>windowsManagementApp-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Entität der Windows-Verwaltungs-app.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsManagementApp abrufen](../api/intune-devices-windowsmanagementapp-get.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Lesen von Eigenschaften und Beziehungen des [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) -Objekts.|
|[WindowsManagementApp aktualisieren](../api/intune-devices-windowsmanagementapp-update.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Aktualisieren der Eigenschaften eines [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutige ID für die Windows-Verwaltungs-App|
|availableVersion|Zeichenfolge|Verfügbare Version der Windows-Verwaltungs-app.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|healthSummary|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)|Integritäts Zusammenfassung für die Windows-Verwaltungs-app.|
|Healthstates wurden|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Sammlung|Die Liste der Integritätsstatus für die installierte Windows-Verwaltungs-app.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "String (identifier)",
  "availableVersion": "String"
}
```




