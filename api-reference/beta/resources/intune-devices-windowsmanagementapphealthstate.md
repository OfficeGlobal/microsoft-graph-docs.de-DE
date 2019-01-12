---
title: Ressourcentyp windowsManagementAppHealthState
description: Windows Management app Health Zustand Entität.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8cf679cf1a5ac86c47354db2fc9f800647d309c1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976471"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a>Ressourcentyp windowsManagementAppHealthState

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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





