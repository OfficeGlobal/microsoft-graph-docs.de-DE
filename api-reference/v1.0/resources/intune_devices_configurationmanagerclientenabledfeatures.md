# <a name="configurationmanagerclientenabledfeatures-resource-type"></a>configurationManagerClientEnabledFeatures-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Im Konfigurations-Manager-Client aktivierte Features
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|inventory|Boolean|Gibt an, ob der Bestand von Intune verwaltet wird|
|modernApps|Boolean|Gibt an, ob die moderne Anwendung von Intune verwaltet wird|
|resourceAccess|Boolean|Gibt an, ob der Zugriff auf Ressourcen von Intune verwaltet wird|
|deviceConfiguration|Boolean|Gibt an, ob die Gerätekonfiguration von Intune verwaltet wird|
|compliancePolicy|Boolean|Gibt an, ob Compliance-Richtlinie von Intune verwaltet wird|
|windowsUpdateForBusiness|Boolean|Gibt an, ob Windows Update for Business von Intune verwaltet wird|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true
}
```


