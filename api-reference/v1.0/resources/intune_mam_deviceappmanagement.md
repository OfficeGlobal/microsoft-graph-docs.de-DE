# <a name="deviceappmanagement-resource-type"></a>deviceAppManagement-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Singleton-Entität für die Geräte-App-Verwaltung
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceAppManagement abrufen](../api/intune_mam_deviceappmanagement_get.md)|[deviceAppManagement](../resources/intune_mam_deviceappmanagement.md)|Lesen von Eigenschaften und Beziehungen des [deviceAppManagement](../resources/intune_mam_deviceappmanagement.md)-Objekts.|
|[deviceAppManagement aktualisieren](../api/intune_mam_deviceappmanagement_update.md)|[deviceAppManagement](../resources/intune_mam_deviceappmanagement.md)|Aktualisieren der Eigenschaften eines [deviceAppManagement](../resources/intune_mam_deviceappmanagement.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|managedAppPolicies|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md)-Sammlung|Richtlinien verwalteter Apps|
|iosManagedAppProtections|[iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md)-Sammlung|Richtlinien verwalteter iOS-Apps|
|androidManagedAppProtections|[androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md)-Sammlung|Richtlinien verwalteter Android-Apps|
|defaultManagedAppProtections|[defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md)-Sammlung|Standardrichtlinien verwalteter Apps|
|targetedManagedAppConfigurations|[targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md)-Sammlung|Zielkonfigurationen verwalteter Apps|
|mdmWindowsInformationProtectionPolicies|[mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md)-Sammlung|Windows Information Protection für Apps auf in MDM registrierten Geräten|
|windowsInformationProtectionPolicies|[windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md)-Sammlung|Windows Information Protection für Apps auf nicht in MDM registrierten Geräten|
|managedAppRegistrations|[managedAppRegistration](../resources/intune_mam_managedappregistration.md)-Sammlung|Die Registrierungen verwalteter Apps|
|managedAppStatuses|[managedAppStatus](../resources/intune_mam_managedappstatus.md)-Sammlung|Die Status der verwalteten Apps|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```



