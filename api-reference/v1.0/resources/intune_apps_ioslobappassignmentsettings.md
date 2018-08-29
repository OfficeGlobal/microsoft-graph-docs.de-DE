# <a name="ioslobappassignmentsettings-resource-type"></a>iosLobAppAssignmentSettings-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Branchen-App zu einer Gruppe.

Erbt von [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|vpnConfigurationId|Zeichenfolge|Die VPN-Konfigurations-ID, die für diese App verwendet wird.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.mobileAppAssignmentSettings",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```



