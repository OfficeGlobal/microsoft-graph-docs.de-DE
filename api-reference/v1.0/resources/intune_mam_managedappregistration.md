# <a name="managedappregistration-resource-type"></a>Ressourcentyp „managedAppRegistration“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Der Entitätstyp „ManagedAppEntity“ ist der Basisentitätstyp für alle anderen Entitätstypen im Workflow für die App-Verwaltung.
Die Ressource „managedAppRegistration“ repräsentiert die Details einer verwalteten App, die von einem Mitglied der Organisation verwendet wird.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „managedAppRegistration](../api/intune_mam_managedappregistration_list.md)|Sammlung von Objekten des Typs [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune_mam_managedappregistration.md) auf.|
|[Abrufen von „managedAppRegistration“](../api/intune_mam_managedappregistration_get.md)|[managedAppRegistration](../resources/intune_mam_managedappregistration.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|[Funktion „getUserIdsWithFlaggedAppRegistration“](../api/intune_mam_managedappregistration_getuseridswithflaggedappregistration.md)|String-Sammlung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung|
|lastSyncDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst|
|applicationVersion|String|Version der App|
|managementSdkVersion|String|Version des App-Verwaltungs-SDK|
|platformVersion|String|Version des Betriebssystems|
|deviceType|String|Gerätetyp des Hostgeräts|
|deviceTag|String|Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden. Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.|
|deviceName|String|Gerätename des Hostgeräts|
|flaggedReasons|String-Sammlung|Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde. Beispiel: Die App wird auf einem gerooteten Gerät ausgeführt.|
|userId|String|Benutzer-ID, zu der die App-Registrierung gehört|
|appIdentifier|[mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)|Bezeichner des App-Pakets|
|id|String|Schlüssel der Entität|
|version|String|Version der Entität|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|appliedPolicies|Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Richtlinien (0 oder mehr), die bereits auf die registrierte App angewendet wurden, als sie letztmals mit dem Verwaltungsdienst synchronisiert wurde|
|intendedPolicies|Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Richtlinien (0 oder mehr), die der Administrator bisher für die App vorgesehen hat|
|operations|Sammlung von Objekten des Typs [managedAppOperation](../resources/intune_mam_managedappoperation.md)|Operationen (0 oder mehr) mit langer Ausführungszeit, die bei der App-Registrierung ausgelöst wurden|

## <a name="json-representation"></a>JSON-Darstellung
Unten sehen Sie eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
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
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```



