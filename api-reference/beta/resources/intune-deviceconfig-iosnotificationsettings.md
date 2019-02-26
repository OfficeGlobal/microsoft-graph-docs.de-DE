---
title: iosNotificationSettings-Ressourcentyp
description: Ein Element zur Beschreibung der Benachrichtigungseinstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2876146e7e20ad94a7356f623a5b2e17443a18f8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172702"
---
# <a name="iosnotificationsettings-resource-type"></a>iosNotificationSettings-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Ein Element zur Beschreibung der Benachrichtigungseinstellungen.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|Paket-ID|Zeichenfolge|Paket-ID der App, auf die diese Benachrichtigungseinstellungen angewandt werden.|
|Anwendungsname|Zeichenfolge|Anwendungsname, der der Paket-ID zugeordnet werden muss.|
|Herausgeber|Zeichenfolge|Herausgeber, der der Paket-ID zugeordnet werden muss.|
|enabled|Boolean|Gibt an, ob Benachrichtigungen für diese App zulässig sind.|
|showInNotificationCenter|Boolean|Gibt an, ob Benachrichtigungen im Nachrichtencenter angezeigt werden können.|
|showOnLockScreen|Boolean|Gibt an, ob Benachrichtigungen auf dem Sperrbildschirm angezeigt werden können.|
|alertType|[iosNotificationAlertType](../resources/intune-deviceconfig-iosnotificationalerttype.md)|Gibt die Art der Warnung für Benachrichtigungen für diese App an. Mögliche Werte: `deviceDefault`, `banner`, `modal`, `none`.|
|badgesEnabled|Boolean|Gibt an, ob Badges für diese App zulässig sind.|
|soundsEnabled|Boolescher Wert|Gibt an, ob Ton für diese App zulässig ist.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true
}
```




