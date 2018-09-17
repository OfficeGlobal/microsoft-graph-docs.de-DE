# <a name="iosmanagedappregistration-resource-type"></a>iosManagedAppRegistration-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Stellt die Synchronisierungsdetails einer iOS-App mit Verwaltungsfunktionen für einen bestimmten Benutzer dar.
Die Ressource „managedAppRegistration“ repräsentiert die Details einer verwalteten App, die von einem Mitglied der Organisation verwendet wird.

Erbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[iosManagedAppRegistrations auflisten](../api/intune_mam_iosmanagedappregistration_list.md)|[iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md)-Sammlung|Listet die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) auf.|
|[iosManagedAppRegistration abrufen](../api/intune_mam_iosmanagedappregistration_get.md)|[iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md)|Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|lastSyncDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|applicationVersion|Zeichenfolge|App-Version. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|managementSdkVersion|Zeichenfolge|Version des App-Verwaltungs-SDK. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|platformVersion|Zeichenfolge|Version des Betriebssystems. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|deviceType|Zeichenfolge|Gerätetyp des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|deviceTag|Zeichenfolge|Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden. Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|deviceName|Zeichenfolge|Gerätename des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|flaggedReasons|[managedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md)-Sammlung|Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde. Z. B. Die App wird auf einem gerooteten Gerät ausgeführt. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|userId|Zeichenfolge|Benutzer-ID, zu der die App-Registrierung gehört. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|appIdentifier|[mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)|Bezeichner des App-Pakets. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|Version|Zeichenfolge|Version der Entität Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|appliedPolicies|Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Richtlinien (0 oder mehr), die bereits auf die registrierte App angewendet wurden, als sie letztmals mit dem Verwaltungsdienst synchronisiert wurde. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|intendedPolicies|Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Richtlinien (0 oder mehr), die der Administrator bisher für die App vorgesehen hat. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|Vorgänge|Sammlung von Objekten des Typs [managedAppOperation](../resources/intune_mam_managedappoperation.md)|Operationen (0 oder mehr) mit langer Ausführungszeit, die bei der App-Registrierung ausgelöst wurden. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedAppRegistration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosManagedAppRegistration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
    "bundleId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [

"Warning: /api-reference/v1.0/resources/intune_mam_androidmanagedappregistration.md/microsoft.graph.androidManagedAppRegistration/appIdentifier:
      Type mismatch between example and table. Parameter name: appIdentifier; example type: (microsoft.graph.androidMobileAppIdentifier); table type: (microsoft.graph.mobileAppIdentifier)",

"Warning: /api-reference/v1.0/resources/intune_mam_androidmanagedappregistration.md/microsoft.graph.androidManagedAppRegistration/flaggedReasons:
      Inconsistent types between parameter (String) and table (Object)",

"Warning: /api-reference/v1.0/resources/intune_mam_iosmanagedappregistration.md/microsoft.graph.iosManagedAppRegistration/appIdentifier:
      Type mismatch between example and table. Parameter name: appIdentifier; example type: (microsoft.graph.iosMobileAppIdentifier); table type: (microsoft.graph.mobileAppIdentifier)",

"Warning: /api-reference/v1.0/resources/intune_mam_iosmanagedappregistration.md/microsoft.graph.iosManagedAppRegistration/flaggedReasons:
      Inconsistent types between parameter (String) and table (Object)"

  ],
}
-->