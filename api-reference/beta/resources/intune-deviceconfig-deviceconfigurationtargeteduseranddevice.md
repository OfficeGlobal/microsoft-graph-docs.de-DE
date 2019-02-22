---
title: deviceConfigurationTargetedUserAndDevice-Ressourcentyp
description: Konflikt Zusammenfassung für eine Reihe von Geräte Konfigurationsrichtlinien.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48d73a532f08b0effb6581373300728ad21c5b37
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144142"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a>deviceConfigurationTargetedUserAndDevice-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Konflikt Zusammenfassung für eine Reihe von Geräte Konfigurationsrichtlinien.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|deviceId|Zeichenfolge|Die ID des Geräts in der einchecken.|
|deviceName|Zeichenfolge|Der Name des Geräts in der einchecken.|
|userId|Zeichenfolge|Die ID des Benutzers in der einchecken.|
|userDisplayName|String|Der Anzeigename des Benutzers in der Einchecken|
|userPrincipalName|String|Der UPN des Benutzers beim Einchecken.|
|lastCheckinDateTime|DateTimeOffset|Letzter Eincheck Zeitpunkt für dieses Benutzer/Gerät-Paar.|

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




