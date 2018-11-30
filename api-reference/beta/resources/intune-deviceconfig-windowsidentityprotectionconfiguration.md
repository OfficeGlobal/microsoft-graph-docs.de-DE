---
title: Ressourcentyp windowsIdentityProtectionConfiguration
description: Diese Entität enthält Beschreibungen der deklarierten Methoden, Eigenschaften und Beziehungen von Windows Hello für Unternehmen verfügbar gemacht werden.
ms.openlocfilehash: 0ac5c291dd85d3ac94378a74ee879bfab2685827
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058116"
---
# <a name="windowsidentityprotectionconfiguration-resource-type"></a>Ressourcentyp windowsIdentityProtectionConfiguration

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Entität enthält Beschreibungen der deklarierten Methoden, Eigenschaften und Beziehungen von Windows Hello für Unternehmen verfügbar gemacht werden.

Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste windowsIdentityProtectionConfigurations](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-list.md)|[WindowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Auflistung|Listeneigenschaften und Beziehungen der [WindowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Objekte.|
|[Abrufen von windowsIdentityProtectionConfiguration](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-get.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Lesen Sie Eigenschaften und Beziehungen des [WindowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Objekts.|
|[Erstellen von windowsIdentityProtectionConfiguration](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-create.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Erstellen eines neuen [WindowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Objekts.|
|[WindowsIdentityProtectionConfiguration löschen](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-delete.md)|Keines|Löscht eine [WindowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).|
|[WindowsIdentityProtectionConfiguration aktualisieren](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-update.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Aktualisieren Sie die Eigenschaften eines [WindowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Collection von Objekten des Typs „String“|Liste der Bereich Tags für diese Instanz der Entität. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolesch|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt. Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden. Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|enhancedAntiSpoofingForFacialFeaturesEnabled|Boolesch|Boolescher Wert verwendet, um erweiterte Anti-spoofing für die Spracherkennung auf Windows Hello Gesicht Authentifizierung Gesichtsausdruck Feature aktivieren.|
|pinMinimumLength|Int32|Integer-Wert, der die Mindestanzahl der Zeichen für den Windows Hello für Business PIN benötigt wird. Gültige Werte sind 4 bis 127 und kleiner als oder gleich dem Wert für die maximale PIN festlegen. Gültige Werte 4 bis 127|
|pinMaximumLength|Int32|Integer-Wert, der die maximale Anzahl der zulässigen Zeichen für die Arbeit PIN festlegt. Gültige Werte sind 4 bis 127 inklusive und größer als oder gleich dem Wert für die minimale PIN festlegen. Gültige Werte 4 bis 127|
|pinUppercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Dieser Wert konfiguriert die Verwendung von Großbuchstaben in der Windows Hello für Business PIN ein. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|pinLowercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Dieser Wert konfiguriert die Verwendung von Kleinbuchstaben in der Windows Hello für Business PIN ein. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|pinSpecialCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Steuert die Möglichkeit, Sonderzeichen in der Windows Hello für Business PIN verwenden. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|pinExpirationInDays|Int32|Integer-Wert gibt den Zeitraum (in Tagen) an, dass eine PIN-Nummer verwendet werden kann, bevor das System den Benutzer es ändern müssen. Gültige Werte sind 0, 730. Gültige Werte: 0 bis 730.|
|pinPreviousBlockCount|Int32|Steuert die Möglichkeit, zu verhindern, dass Benutzer die ältere PINs verwenden. Dies muss zwischen 0 und 50, einschließlich festgelegt werden, und die aktuelle PIN des Benutzers in diese Zählung eingeschlossen ist. Wenn auf 0 gesetzt, vorherigen PINs nicht gespeichert werden. PIN-Verlauf wird nicht beibehalten, über eine PIN zurücksetzen. Gültige Werte: 0 bis 50.|
|pinRecoveryEnabled|Boolesch|Boolescher Wert, mit der einen Benutzer seine PIN mithilfe der Windows Hello für Recovery-Service Business PIN ändern kann.|
|securityDeviceRequired|Boolescher Wert|Steuert, ob ein vertrauenswürdiger Platform-Modul (TPM) für die Bereitstellung von Windows Hello für Unternehmen erforderlich ist. Ein TPM bietet einen zusätzliche Sicherheit-Vorteil, dass darauf gespeicherte Daten auf anderen Geräten verwendet werden können. Wenn auf False festgelegt, alle Geräte Windows Hello für Unternehmen bereitstellen können, auch wenn ein verwendbar TPM nicht vorhanden ist.|
|unlockWithBiometricsEnabled|Boolescher Wert|Steuert die Verwendung von biometrische Gesten, wie das Standardsymbol zurück und Fingerabdruck, als Alternative zu den Windows Hello für Business PIN an.  Wenn es sich bei Festlegung auf "false", biometrische Gesten nicht zulässig sind. Benutzer müssen eine PIN weiterhin als Sicherungskopie bei Fehlern konfigurieren.|
|useCertificatesForOnPremisesAuthEnabled|Boolesch|Boolescher Wert, mit der Windows Hello für Unternehmen von Zertifikaten auf Standortbasierte Ressourcen authentifizieren kann.|
|windowsHelloForBusinessBlocked|Boolescher Wert|Boolescher Wert, der Windows Hello für Unternehmen als Methode für die Anmeldung bei Windows blockiert.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Auflistung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung|Gerät Konfiguration Installationsstatus durch Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries| [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsIdentityProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 1024,
  "pinMaximumLength": 1024,
  "pinUppercaseCharactersUsage": "String",
  "pinLowercaseCharactersUsage": "String",
  "pinSpecialCharactersUsage": "String",
  "pinExpirationInDays": 1024,
  "pinPreviousBlockCount": 1024,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```





