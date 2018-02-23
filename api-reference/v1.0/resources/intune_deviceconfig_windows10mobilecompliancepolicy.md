# <a name="windows10mobilecompliancepolicy-resource-type"></a>windows10MobileCompliancePolicy-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Klasse enthält Konformitätseinstellungen für Windows 10 Mobile.

Sie erbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[windows10MobileCompliancePolicies auflisten](../api/intune_deviceconfig_windows10mobilecompliancepolicy_list.md)|[windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md)-Sammlung|Listet die Eigenschaften und Beziehungen von Objekten des Typs [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) auf.|
|[windows10MobileCompliancePolicy abrufen](../api/intune_deviceconfig_windows10mobilecompliancepolicy_get.md)|[windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md)|Lesen von Eigenschaften und Beziehungen des [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md)-Objekts.|
|[windows10MobileCompliancePolicy erstellen](../api/intune_deviceconfig_windows10mobilecompliancepolicy_create.md)|[windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md)|Erstellen eines neuen [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md)-Objekts.|
|[windows10MobileCompliancePolicy löschen](../api/intune_deviceconfig_windows10mobilecompliancepolicy_delete.md)|Keine|Löscht eine [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md).|
|[windows10MobileCompliancePolicy aktualisieren](../api/intune_deviceconfig_windows10mobilecompliancepolicy_update.md)|[windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md)|Aktualisiert die Eigenschaften von Objekten des Typs [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|passwordRequired|Boolescher Wert|Legt fest, dass zum Entsperren des Windows Phone-Geräts ein Kennwort erforderlich ist.|
|passwordBlockSimple|Boolescher Wert|Gibt an, ob die Kalendersynchronisierung blockiert werden soll.|
|passwordMinimumLength|Int32|Mindestlänge des Kennworts. Gültige Werte: 4 bis 16.|
|passwordMinimumCharacterSetCount|Int32|Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen|
|passwordRequiredType|Zeichenfolge|Geforderter Kennworttyp. Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.|
|passwordPreviousPasswordBlockCount|Int32|Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.|
|passwordExpirationDays|Int32|Zeit in Tagen bis zum Ablaufen des Kennworts. Gültige Werte: 1 bis 255.|
|passwordMinutesOfInactivityBeforeLock|Int32|Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird|
|passwordRequireToUnlockFromIdle|Boolescher Wert|Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.|
|osMinimumVersion|Zeichenfolge|Mindestversion von Windows Phone|
|osMaximumVersion|Zeichenfolge|Maximalversion von Windows Phone|
|earlyLaunchAntiMalwareDriverEnabled|Boolescher Wert|Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.|
|bitLockerEnabled|Boolescher Wert|Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.|
|secureBootEnabled|Boolescher Wert|Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.|
|codeIntegrityEnabled|Boolescher Wert|Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.|
|storageRequireEncryption|Boolescher Wert|Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|scheduledActionsForRule|Sammlung von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|Liste der geplanten Aktionen für die Regel. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|deviceStatuses|Sammlung von Objekten des Typs [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md)|Liste von Objekten des Typs „deviceComplianceDeviceStatus“. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|userStatuses|Sammlung von Objekten des Typs [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|Liste von Objekten des Typs „deviceComplianceUserStatus“. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|Übersicht über den Status der Gerätekonformität nach Gerät. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|Übersicht über den Status der Gerätekonformität nach Benutzer. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|deviceSettingStateSummaries|Sammlung von Objekten des Typs [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Übersicht über den Einstellungsstatus der Konformitätsrichtlinie nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|assignments|Sammlung von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|Sammlung von Zuweisungen für die Konformitätsrichtlinie. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10MobileCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordExpirationDays": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```



