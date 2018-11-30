---
title: Ressourcentyp deviceConfigurationTargetedUserAndDevice
description: Zusammenfassung für einen Satz von Richtlinien für die Konfiguration von Geräte Konflikt.
ms.openlocfilehash: 6f79a8fe24e06d2bdafa81c30cabf8158b4e5773
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058980"
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





