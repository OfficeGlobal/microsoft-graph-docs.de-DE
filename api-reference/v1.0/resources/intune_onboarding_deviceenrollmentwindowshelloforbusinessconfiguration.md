# <a name="deviceenrollmentwindowshelloforbusinessconfiguration-resource-type"></a>deviceEnrollmentWindowsHelloForBusinessConfiguration-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert.

Erbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DeviceEnrollmentWindowsHelloForBusinessConfigurations auflisten](../api/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration_list.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekte.|
|[DeviceEnrollmentWindowsHelloForBusinessConfiguration abrufen](../api/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration_get.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.|
|[DeviceEnrollmentWindowsHelloForBusinessConfiguration erstellen](../api/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration_create.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)|Erstellen eines neuen [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.|
|[DeviceEnrollmentWindowsHelloForBusinessConfiguration löschen](../api/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration_delete.md)|Keine|Löscht ein [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekt.|
|[DeviceEnrollmentWindowsHelloForBusinessConfiguration aktualisieren](../api/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration_update.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)|Aktualisieren der Eigenschaften eines [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|
|displayName|String|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|
|description|String|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|
|priority|Int32|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|
|version|Int32|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|
|pinMinimumLength|Int32|Noch nicht dokumentiert.|
|pinMaximumLength|Int32|Noch nicht dokumentiert.|
|pinUppercaseCharactersUsage|String|Noch nicht dokumentiert. Mögliche Werte: `allowed`, `required`, `disallowed`.|
|pinLowercaseCharactersUsage|String|Noch nicht dokumentiert. Mögliche Werte: `allowed`, `required`, `disallowed`.|
|pinSpecialCharactersUsage|String|Noch nicht dokumentiert. Mögliche Werte: `allowed`, `required`, `disallowed`.|
|state|String|Noch nicht dokumentiert. Mögliche Werte: `notConfigured`, `enabled`, `disabled`.|
|securityDeviceRequired|Boolean|Noch nicht dokumentiert.|
|unlockWithBiometricsEnabled|Boolean|Noch nicht dokumentiert.|
|remotePassportEnabled|Boolean|Noch nicht dokumentiert.|
|pinPreviousBlockCount|Int32|Noch nicht dokumentiert.|
|pinExpirationInDays|Int32|Noch nicht dokumentiert.|
|enhancedBiometricsState|String|Noch nicht dokumentiert. Mögliche Werte: `notConfigured`, `enabled`, `disabled`.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)-Sammlung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "pinMinimumLength": 1024,
  "pinMaximumLength": 1024,
  "pinUppercaseCharactersUsage": "String",
  "pinLowercaseCharactersUsage": "String",
  "pinSpecialCharactersUsage": "String",
  "state": "String",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 1024,
  "pinExpirationInDays": 1024,
  "enhancedBiometricsState": "String"
}
```



