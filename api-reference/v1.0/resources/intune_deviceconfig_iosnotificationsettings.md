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
|alertType|Zeichenfolge|Gibt die Art der Warnung für Benachrichtigungen für diese App an. Mögliche Werte: `deviceDefault`, `banner`, `modal`, `none`.|
|badgesEnabled|Boolescher Wert|Gibt an, ob Badges für diese App zulässig sind.|
|soundsEnabled|Boolescher Wert|Gibt an, ob Ton für diese App zulässig ist.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



