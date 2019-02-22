---
title: windowsManagementAppHealthState-Ressourcentyp
description: Integritätszustands Entität der Windows-Verwaltungs app.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8841b79b9a284a15999db701e82a2b5062e2930b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148538"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a>windowsManagementAppHealthState-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Integritätszustands Entität der Windows-Verwaltungs app.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsManagementAppHealthStates aufListen](../api/intune-devices-windowsmanagementapphealthstate-list.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekte.|
|[WindowsManagementAppHealthState abrufen](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Lesen von Eigenschaften und Beziehungen des [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekts.|
|[WindowsManagementAppHealthState erstellen](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Erstellen eines neuen [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekts.|
|[WindowsManagementAppHealthState löschen](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|Keine|Löscht eine [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).|
|[WindowsManagementAppHealthState aktualisieren](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Aktualisieren der Eigenschaften eines [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für den Integritätsstatus der Windows-Verwaltungsanwendung|
|healthState|[healthState](../resources/intune-devices-healthstate.md)|Integritätsstatus der Windows-Verwaltungsanwendung Mögliche Werte sind: `unknown`, `healthy` und `unhealthy`.|
|installedVersion|Zeichenfolge|Installierte Version der Windows-Verwaltungs-app.|
|lastCheckInDateTime|DateTimeOffset|Windows Management APP – letzter Eincheck Zeitpunkt.|
|deviceName|Zeichenfolge|Name des Geräts, auf dem die Windows-Verwaltungs-App installiert ist.|
|deviceOSVersion|Zeichenfolge|Windows 10-Betriebssystemversion des Geräts, auf dem die Windows-Verwaltungs-App installiert ist.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "String (identifier)",
  "healthState": "String",
  "installedVersion": "String",
  "lastCheckInDateTime": "String (timestamp)",
  "deviceName": "String",
  "deviceOSVersion": "String"
}
```




