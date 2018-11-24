# <a name="windows81compliancepolicy-resource-type"></a>Ressourcentyp „windows81CompliancePolicy“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Klasse enthält Konformitätseinstellungen für Windows 8.1.

Sie erbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „windows81CompliancePolicies“](../api/intune_deviceconfig_windows81compliancepolicy_list.md)|Sammlung von Objekten des Typs [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) auf.|
|[Abrufen von „windows81CompliancePolicy“](../api/intune_deviceconfig_windows81compliancepolicy_get.md)|[windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md).|
|[Erstellen von „windows81CompliancePolicy“](../api/intune_deviceconfig_windows81compliancepolicy_create.md)|[windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md)|Erstellt neue Objekte des Typs [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md).|
|[Löschen von „windows81CompliancePolicy“](../api/intune_deviceconfig_windows81compliancepolicy_delete.md)|Keiner|Löscht Objekte des Typs [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md).|
|[Aktualisieren von „windows81CompliancePolicy“](../api/intune_deviceconfig_windows81compliancepolicy_update.md)|[windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md)|Aktualisiert die Eigenschaften von Objekten des Typs [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|passwordRequired|Boolean|Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.|
|passwordBlockSimple|Boolean|Gibt an, ob einfache Kennwörter erlaubt sind.|
|passwordExpirationDays|Int32|Zeit bis zum Ablaufen des Kennworts in Tagen|
|passwordMinimumLength|Int32|Mindestlänge des Kennworts|
|passwordMinutesOfInactivityBeforeLock|Int32|Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird|
|passwordMinimumCharacterSetCount|Int32|Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen.|
|passwordRequiredType|[requiredPasswordType](../resources/intune_deviceconfig_requiredpasswordtype.md)|Geforderter Kennworttyp. Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.|
|passwordPreviousPasswordBlockCount|Int32|Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss. Gültige Werte: 0 bis 24.|
|osMinimumVersion|String|Mindestversion von Windows 8.1|
|osMaximumVersion|String|Maximalversion von Windows 8.1|
|storageRequireEncryption|Boolean|Gibt an, ob für ein Windows 8.1-Gerät Verschlüsselung gefordert wird.|

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
Unten sehen Sie eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows81CompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "passwordPreviousPasswordBlockCount": 1024,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "storageRequireEncryption": true
}
```



