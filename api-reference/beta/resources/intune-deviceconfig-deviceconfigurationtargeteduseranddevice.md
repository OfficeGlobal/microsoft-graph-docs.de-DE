---
title: Ressourcentyp deviceConfigurationTargetedUserAndDevice
description: Zusammenfassung für einen Satz von Richtlinien für die Konfiguration von Geräte Konflikt.
author: tfitzmac
ms.openlocfilehash: 04b0e31d0f3f099389e4901eb654139d286f4bd8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345241"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a>Ressourcentyp deviceConfigurationTargetedUserAndDevice

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Zusammenfassung für einen Satz von Richtlinien für die Konfiguration von Geräte Konflikt.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|deviceId|String|Die Id des Geräts in das Einchecken.|
|deviceName|String|Der Name des Geräts in das Einchecken.|
|userId|String|Die Id des Benutzers in das Einchecken.|
|userDisplayName|String|Der Anzeigename des Benutzers in das Einchecken|
|userPrincipalName|String|Den UPN des Benutzers in das Einchecken.|
|lastCheckinDateTime|DateTimeOffset|Zeitpunkt der letzten Checkin für diese Benutzer/Geräte-Paar.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationTargetedUserAndDevice",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "lastCheckinDateTime": "String (timestamp)"
}
```





