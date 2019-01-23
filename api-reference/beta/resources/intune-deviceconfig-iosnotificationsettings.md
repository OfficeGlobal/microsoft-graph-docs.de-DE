---
title: iosNotificationSettings-Ressourcentyp
description: Ein Element zur Beschreibung der Benachrichtigungseinstellungen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7db0b6ba438522db0795f6897daba8b5c43258c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420500"
---
# <a name="iosnotificationsettings-resource-type"></a>iosNotificationSettings-Ressourcentyp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Ein Element zur Beschreibung der Benachrichtigungseinstellungen.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|Paket-ID|Zeichenfolge|Paket-ID der App, auf die diese Benachrichtigungseinstellungen angewandt werden.|
|Anwendungsname|Zeichenfolge|Anwendungsname, der der Paket-ID zugeordnet werden muss.|
|Herausgeber|Zeichenfolge|Herausgeber, der der Paket-ID zugeordnet werden muss.|
|enabled|Boolescher Wert|Gibt an, ob Benachrichtigungen für diese App zulässig sind.|
|showInNotificationCenter|Boolescher Wert|Gibt an, ob Benachrichtigungen im Nachrichtencenter angezeigt werden können.|
|showOnLockScreen|Boolescher Wert|Gibt an, ob Benachrichtigungen auf dem Sperrbildschirm angezeigt werden können.|
|alertType|[iosNotificationAlertType](../resources/intune-deviceconfig-iosnotificationalerttype.md)|Gibt die Art der Warnung für Benachrichtigungen für diese App an. Mögliche Werte: `deviceDefault`, `banner`, `modal`, `none`.|
|badgesEnabled|Boolescher Wert|Gibt an, ob Badges für diese App zulässig sind.|
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




