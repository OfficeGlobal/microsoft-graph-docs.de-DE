---
title: Ressourcentyp windowsManagementAppHealthState
description: Windows Management app Health Zustand Entität.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 171ae2492eb5077567f4398af678d14044a0b7e2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395734"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a>Ressourcentyp windowsManagementAppHealthState

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Windows Management app Health Zustand Entität.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste windowsManagementAppHealthStates](../api/intune-devices-windowsmanagementapphealthstate-list.md)|[WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Auflistung|Listeneigenschaften und Beziehungen der [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekte.|
|[Abrufen von windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Lesen Sie Eigenschaften und Beziehungen des [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekts.|
|[Erstellen von windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Erstellen eines neuen [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekts.|
|[WindowsManagementAppHealthState löschen](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|Keine|Löscht eine [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).|
|[WindowsManagementAppHealthState aktualisieren](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Aktualisieren Sie die Eigenschaften eines [WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für den Zustand des Windows Management-app|
|healthState|[healthState](../resources/intune-devices-healthstate.md)|Windows Management app Zustand. Mögliche Werte sind: `unknown`, `healthy` und `unhealthy`.|
|installedVersion|Zeichenfolge|Windows Management-app-Version installiert.|
|lastCheckInDateTime|DateTimeOffset|Windows Management app Einchecken zuletzt.|
|deviceName|Zeichenfolge|Name des Geräts, auf dem Windows Management-app installiert ist.|
|deviceOSVersion|Zeichenfolge|Windows 10 Betriebssystemversion des Geräts, auf dem Windows Management-app installiert ist.|

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




