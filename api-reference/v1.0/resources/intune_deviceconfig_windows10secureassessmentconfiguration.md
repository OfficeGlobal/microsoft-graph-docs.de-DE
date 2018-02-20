# <a name="windows10secureassessmentconfiguration-resource-type"></a>Ressourcentyp „windows10SecureAssessmentConfiguration“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „secureAssessment“ verfügbar gemacht werden.

Sie erbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „windows10SecureAssessmentConfiguration“](../api/intune_deviceconfig_windows10secureassessmentconfiguration_list.md)|Sammlung von Objekten des Typs [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) auf.|
|[Abrufen von „windows10SecureAssessmentConfiguration“](../api/intune_deviceconfig_windows10secureassessmentconfiguration_get.md)|[windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md).|
|[Erstellen von „windows10SecureAssessmentConfiguration“](../api/intune_deviceconfig_windows10secureassessmentconfiguration_create.md)|[windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md)|Erstellt neue Objekte des Typs [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md).|
|[Löschen von „windows10SecureAssessmentConfiguration“](../api/intune_deviceconfig_windows10secureassessmentconfiguration_delete.md)|Keiner|Löscht neue Objekte des Typs [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md).|
|[Aktualisieren von „windows10SecureAssessmentConfiguration“](../api/intune_deviceconfig_windows10secureassessmentconfiguration_update.md)|[windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md)|Aktualisiert die Eigenschaften von Objekten des Typs [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|launchUri|String|URL zu einer Bewertung, die automatisch geladen wird, sobald der Browser für sichere Bewertungen gestartet wird. Die URL muss eine gültige URL sein (http\[s\]://msdn.microsoft.com/).|
|configurationAccount|String|Konto, mit dem das Windows-Gerät für den Test konfiguriert wurde. Der Benutzer kann ein Domänenkonto (Domäne\Benutzername), ein AAD-Konto (benutzername@mandant.com) oder ein lokales Konto (Benutzername) sein.|
|allowPrinting|Boolean|Gibt an, ob während des Tests über die App gedruckt werden darf.|
|allowScreenCapture|Boolean|Gibt an, ob während des Tests über die App Screenshots angefertigt werden dürfen.|
|allowTextSuggestion|Boolean|Gibt an, ob während des Tests Wortvorschläge angezeigt werden dürfen.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|Sammlung von Objekten des Typs [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatuses|Sammlung von Objekten des Typs [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatuses|Sammlung von Objekten des Typs [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceSettingStateSummaries|Sammlung von Objekten des Typs [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Unten sehen Sie eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10SecureAssessmentConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "launchUri": "String",
  "configurationAccount": "String",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```


