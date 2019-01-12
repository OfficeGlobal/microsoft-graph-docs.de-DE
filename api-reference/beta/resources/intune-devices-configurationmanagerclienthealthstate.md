---
title: Ressourcentyp configurationManagerClientHealthState
description: Konfigurations-Manager-Client-Zustand
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4d202b5f672977e8bb1a5fe05ba56937005825ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981742"
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





