---
title: Ressourcentyp deviceConfigurationTargetedUserAndDevice
description: Zusammenfassung für einen Satz von Richtlinien für die Konfiguration von Geräte Konflikt.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 46355f78f23060ecc901c3f98f0e3f7d13101d1e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809625"
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





