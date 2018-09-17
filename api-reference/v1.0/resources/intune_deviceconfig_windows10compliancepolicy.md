# <a name="windows10compliancepolicy-resource-type"></a>Ressourcentyp „windows10CompliancePolicy“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Klasse enthält Konformitätseinstellungen für Windows 10.

Sie erbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „windows10CompliancePolicy“](../api/intune_deviceconfig_windows10compliancepolicy_list.md)|Sammlung von Objekten des Typs [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) auf.|
|[Abrufen von „windows10CompliancePolicy“](../api/intune_deviceconfig_windows10compliancepolicy_get.md)|[windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).|
|[Erstellen von „windows10CompliancePolicy“](../api/intune_deviceconfig_windows10compliancepolicy_create.md)|[windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md)|Erstellt neue Objekte des Typs [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).|
|[Löschen von „windows10CompliancePolicy“](../api/intune_deviceconfig_windows10compliancepolicy_delete.md)|Keiner|Löscht Objekte des Typs [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).|
|[Aktualisieren von „windows10CompliancePolicy“](../api/intune_deviceconfig_windows10compliancepolicy_update.md)|[windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md)|Aktualisiert die Eigenschaften von Objekten des Typs [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|Schlüssel der Entität Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|Beschreibung|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|passwordRequired|Boolesch|Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.|
|passwordBlockSimple|Boolesch|Gibt an, ob einfache Kennwörter erlaubt sind.|
|passwordRequiredToUnlockFromIdle|Boolesch|Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.|
|passwordMinutesOfInactivityBeforeLock|Int32|Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird|
|passwordExpirationDays|Int32|Zeitraum in Tagen bis zum Ablaufen des Kennworts|
|passwordMinimumLength|Int32|Mindestlänge des Kennworts|
|passwordMinimumCharacterSetCount|Int32|Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen|
|passwordRequiredType|[requiredPasswordType](../resources/intune_deviceconfig_requiredpasswordtype.md)|Geforderter Kennworttyp. Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.|
|passwordPreviousPasswordBlockCount|Int32|Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.|
|requireHealthyDeviceReport|Boolesch|Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.|
|osMinimumVersion|Zeichenfolge|Mindestversion von Windows 10|
|osMaximumVersion|Zeichenfolge|Maximalversion von Windows 10|
|mobileOsMinimumVersion|Zeichenfolge|Mindestversion von Windows Phone|
|mobileOsMaximumVersion|Zeichenfolge|Maximalversion von Windows Phone|
|earlyLaunchAntiMalwareDriverEnabled|Boolesch|Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.|
|bitLockerEnabled|Boolesch|Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.|
|secureBootEnabled|Boolesch|Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.|
|codeIntegrityEnabled|Boolesch|Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.|
|storageRequireEncryption|Boolesch|Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|scheduledActionsForRule|Sammlung von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|Liste der geplanten Aktionen für die Regel. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|deviceStatuses|Sammlung von Objekten des Typs [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md)|Liste von Objekten des Typs „deviceComplianceDeviceStatus“. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|userStatuses|Sammlung von Objekten des Typs [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|Liste von Objekten des Typs „deviceComplianceUserStatus“. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|Übersicht über den Status der Gerätekonformität nach Gerät. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|Übersicht über den Status der Gerätekonformität nach Benutzer. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus der Konformitätsrichtlinie nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|Aufgaben|Sammlung von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|Sammlung von Zuweisungen für die Konformitätsrichtlinie. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceCompliancePolicy",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10CompliancePolicy"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "passwordPreviousPasswordBlockCount": 1024,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "mobileOsMinimumVersion": "String",
  "mobileOsMaximumVersion": "String",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```








