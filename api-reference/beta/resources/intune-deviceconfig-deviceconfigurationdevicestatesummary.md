---
title: deviceConfigurationDeviceStateSummary-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: 7e34420c8ac7c4c05d0eff38d68844b49cd2376d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061598"
---
# <a name="deviceconfigurationdevicestatesummary-resource-type"></a>deviceConfigurationDeviceStateSummary-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceConfigurationDeviceStateSummary abrufen](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-get.md)|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|Lesen von Eigenschaften und Beziehungen des [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)-Objekts.|
|[deviceConfigurationDeviceStateSummary aktualisieren](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-update.md)|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|Aktualisieren der Eigenschaften eines [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|unknownDeviceCount|Int32|Anzahl von unbekannten Geräten|
|notApplicableDeviceCount|Int32|Anzahl der ausgenommenen Geräte|
|compliantDeviceCount|Int32|Anzahl von konformen Geräten|
|remediatedDeviceCount|Int32|Anzahl von korrigierten Geräten|
|nonCompliantDeviceCount|Int32|Anzahl von nicht konformen Geräten|
|errorDeviceCount|Int32|Anzahl von Geräten mit Fehlern|
|conflictDeviceCount|Int32|Anzahl der Geräte mit Konflikten|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```





