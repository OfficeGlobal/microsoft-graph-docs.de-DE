# <a name="windowsphone81compliancepolicy-resource-type"></a>windowsPhone81CompliancePolicy-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Klasse enthält Konformitätseinstellungen für Windows 8.1 Mobile.

Sie erbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsPhone81CompliancePolicies auflisten](../api/intune_deviceconfig_windowsphone81compliancepolicy_list.md)|[windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md)-Objekte.|
|[WindowsPhone81CompliancePolicy abrufen](../api/intune_deviceconfig_windowsphone81compliancepolicy_get.md)|[windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md)|Lesen von Eigenschaften und Beziehungen des [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md)-Objekts.|
|[WindowsPhone81CompliancePolicy erstellen](../api/intune_deviceconfig_windowsphone81compliancepolicy_create.md)|[windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md)|Erstellen eines neuen [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md)-Objekts.|
|[WindowsPhone81CompliancePolicy löschen](../api/intune_deviceconfig_windowsphone81compliancepolicy_delete.md)|Keine|Löscht ein [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md)-Objekt.|
|[WindowsPhone81CompliancePolicy aktualisieren](../api/intune_deviceconfig_windowsphone81compliancepolicy_update.md)|[windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md)|Aktualisieren der Eigenschaften eines [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|description|String|Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|displayName|String|Vom Administrator bereitgestellter Name der Gerätekonfiguration Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|version|Int32|Version der Gerätekonfiguration Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|passwordBlockSimple|Boolean|Gibt an, ob die Kalendersynchronisierung blockiert werden soll.|
|passwordExpirationDays|Int32|Zeit in Tagen bis zum Ablaufen des Kennworts|
|passwordMinimumLength|Int32|Mindestlänge von Kennwörtern|
|passwordMinutesOfInactivityBeforeLock|Int32|Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird|
|passwordMinimumCharacterSetCount|Int32|Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen|
|passwordRequiredType|String|Geforderter Kennworttyp. Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.|
|passwordPreviousPasswordBlockCount|Int32|Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen. Gültige Werte: 0 bis 24.|
|passwordRequired|Boolean|Legt fest, ob ein Kennwort gefordert wird.|
|osMinimumVersion|String|Mindestversion von Windows Phone|
|osMaximumVersion|String|Maximalversion von Windows Phone|
|storageRequireEncryption|Boolean|Verschlüsselung auf Windows Phone-Geräten erforderlich|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|scheduledActionsForRule|Sammlung von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|Liste der geplanten Aktionen für die Regel. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|deviceStatuses|Sammlung von Objekten des Typs [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md)|Liste von Objekten des Typs „deviceComplianceDeviceStatus“. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|userStatuses|Sammlung von Objekten des Typs [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|Liste von Objekten des Typs „deviceComplianceUserStatus“. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|Übersicht über den Status der Gerätekonformität nach Gerät. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|Übersicht über den Status der Gerätekonformität nach Benutzer. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|deviceSettingStateSummaries| [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus der Konformitätsrichtlinie nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|assignments|Sammlung von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|Sammlung von Zuweisungen für die Konformitätsrichtlinie. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPhone81CompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequired": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "storageRequireEncryption": true
}
```



