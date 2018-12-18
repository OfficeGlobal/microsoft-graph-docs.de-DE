---
title: iosNotificationSettings-Ressourcentyp
description: Ein Element zur Beschreibung der Benachrichtigungseinstellungen.
author: tfitzmac
ms.openlocfilehash: 197de8b9cd59d1f6c998f92460e62aab480ef455
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307840"
---
# <a name="iosnotificationsettings-resource-type"></a>iosNotificationSettings-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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



