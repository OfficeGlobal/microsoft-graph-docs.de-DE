---
title: Ressourcentyp configurationManagerClientHealthState
description: Konfigurations-Manager-Client-Zustand
author: tfitzmac
ms.openlocfilehash: 8361d74f675cf1eaf70b78e2350aae2fc6e83554
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302786"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a>Ressourcentyp configurationManagerClientHealthState

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Konfigurations-Manager-Client-Zustand
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|state|[configurationManagerClientState](../resources/intune-devices-configurationmanagerclientstate.md)|Aktuelle Configuration Manager-Client-Zustand. Mögliche Werte sind: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed` und `communicationError`.|
|errorCode|Int32|Der Fehlercode für ausgefallenen Zustand.|
|lastSyncDateTime|DateTimeOffset|Zeigen Sie DateTime fo letzte Synchronisierung mit Configuration Manager-Management.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientHealthState",
  "state": "String",
  "errorCode": 1024,
  "lastSyncDateTime": "String (timestamp)"
}
```





