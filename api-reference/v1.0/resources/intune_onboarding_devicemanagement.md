# <a name="devicemanagement-resource-type"></a>deviceManagement-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Singleton-Entität, die als Container für alle Geräteverwaltungsfunktionen dient.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceManagement abrufen](../api/intune_onboarding_devicemanagement_get.md)|[deviceManagement](../resources/intune_onboarding_devicemanagement.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune_onboarding_devicemanagement.md)-Objekts.|
|[deviceManagement aktualisieren](../api/intune_onboarding_devicemanagement_update.md)|[deviceManagement](../resources/intune_onboarding_devicemanagement.md)|Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune_onboarding_devicemanagement.md)-Objekts.|
|[verifyWindowsEnrollmentAutoDiscovery-Funktion](../api/intune_onboarding_devicemanagement_verifywindowsenrollmentautodiscovery.md)|Boolescher Wert|Noch nicht dokumentiert.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Noch nicht dokumentiert.|
|intuneBrand|[intuneBrand](../resources/intune_onboarding_intunebrand.md)|„intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|deviceCategories|[deviceCategory](../resources/intune_onboarding_devicecategory.md)-Sammlung|Die Liste der Gerätekategorien mit dem Mandanten.|
|exchangeConnectors|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)-Sammlung|Die Liste der vom Mandanten konfigurierten Exchange-Connectors.|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)-Sammlung|Die Liste der Konfigurationen der Geräteregistrierung.|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|Die Exchange-Einstellungen für den lokalen, bedingten Zugriff. Für den lokalen, bedingten Zugriff müssen Geräte registriert und für den E-Mail-Zugriff kompatibel sein.|
|mobileThreatDefenseConnectors|[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)-Sammlung|Die Liste der vom Mandanten konfigurierten MTD-Connectors (Mobile Threat Defense).|
|deviceManagementPartners|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)-Sammlung|Die Liste der vom Mandanten konfigurierten Geräteverwaltungspartner.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "intuneBrand": {
    "@odata.type": "microsoft.graph.intuneBrand",
    "displayName": "String",
    "contactITName": "String",
    "contactITPhoneNumber": "String",
    "contactITEmailAddress": "String",
    "contactITNotes": "String",
    "privacyUrl": "String",
    "onlineSupportSiteUrl": "String",
    "onlineSupportSiteName": "String",
    "themeColor": {
      "@odata.type": "microsoft.graph.rgbColor",
      "r": 1024,
      "g": 1024,
      "b": 1024
    },
    "showLogo": true,
    "lightBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "String",
      "value": "binary"
    },
    "darkBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "String",
      "value": "binary"
    },
    "showNameNextToLogo": true,
    "showDisplayNameNextToLogo": true
  }
}
```



