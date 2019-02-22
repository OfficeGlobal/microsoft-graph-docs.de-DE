---
title: windowsIdentityProtectionConfiguration-Ressourcentyp
description: Diese Entität enthält Beschreibungen der deklarierten Methoden, Eigenschaften und Beziehungen, die von Windows Hello for Business verfügbar gemacht werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29510dca8eac2713576f847485a9d22d0bedf1d6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168012"
---
# <a name="windowsidentityprotectionconfiguration-resource-type"></a>windowsIdentityProtectionConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Diese Entität enthält Beschreibungen der deklarierten Methoden, Eigenschaften und Beziehungen, die von Windows Hello for Business verfügbar gemacht werden.


Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsIdentityProtectionConfigurations aufListen](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-list.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Objekte.|
|[WindowsIdentityProtectionConfiguration abrufen](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-get.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Objekts.|
|[WindowsIdentityProtectionConfiguration erstellen](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-create.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Erstellen eines neuen [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Objekts.|
|[WindowsIdentityProtectionConfiguration löschen](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-delete.md)|Keine|Löscht eine [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).|
|[WindowsIdentityProtectionConfiguration aktualisieren](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-update.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Aktualisieren der Eigenschaften eines [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolescher Wert|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|useSecurityKeyForSignin|Boolescher Wert|Boolescher Wert, der zum Aktivieren des Windows Hello-Sicherheitsschlüssels als Anmeldeinformationen verwendet wird.|
|enhancedAntiSpoofingForFacialFeaturesEnabled|Boolescher Wert|Boolescher Wert, mit dem Enhanced Anti-Spoofing für die Erkennung von gesichtsfunktionen unter Windows Hello Face Authentication aktiviert wird.|
|pinMinimumLength|Int32|Ganzzahliger Wert, der die Mindestanzahl von Zeichen für die Windows-Hello for Business-PIN festlegt. Gültige Werte sind 4 bis 127 inklusive und kleiner als oder gleich dem Wert, der für die maximale PIN festgelegt ist. Gültige Werte 4 bis 127|
|pinMaximumLength|Int32|Ganzzahliger Wert, der die maximale Anzahl der zulässigen Zeichen für die Arbeits-PIN festlegt. Gültige Werte sind 4 bis 127 inklusive und größer oder gleich dem Wert, der für die minimale PIN festgelegt ist. Gültige Werte 4 bis 127|
|pinUppercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Dieser Wert konfiguriert die Verwendung von Großbuchstaben in der Windows Hello for Business-PIN. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|pinLowercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Dieser Wert konfiguriert die Verwendung von Kleinbuchstaben in der Windows Hello for Business-PIN. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|pinSpecialCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Steuert die Möglichkeit, Sonderzeichen in der Windows Hello for Business-PIN zu verwenden. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|pinExpirationInDays|Int32|Ganzzahliger Wert gibt den Zeitraum (in Tagen) an, an dem eine PIN verwendet werden kann, bevor das System den Benutzer zum Ändern benötigt. Gültige Werte sind 0 bis 730 inklusive. Gültige Werte: 0 bis 730.|
|pinPreviousBlockCount|Int32|Steuert, wie verhindert werden kann, dass Benutzer frühere PINs verwenden. Dieser muss zwischen 0 und 50 einschließlich festgelegt werden, und die aktuelle PIN des Benutzers ist in dieser Anzahl enthalten. Bei Festlegung auf 0 werden frühere PINs nicht gespeichert. Der PIN-Verlauf wird nicht durch eine PIN-Zurücksetzung beibehalten. Gültige Werte: 0 bis 50.|
|pinRecoveryEnabled|Boolescher Wert|Boolescher Wert, der es einem Benutzer ermöglicht, seine PIN mithilfe des Windows Hello for Business-PIN-Wiederherstellungs Diensts zu ändern.|
|securityDeviceRequired|Boolescher Wert|Steuert, ob ein Trusted Platform Module (TPM) für die Einrichtung von Windows Hello for Business erforderlich ist. Ein TPM bietet einen zusätzlichen Sicherheitsvorteil, da darin gespeicherte Daten nicht auf anderen Geräten verwendet werden können. Wenn dieser Wert auf false festgelegt ist, können alle Geräte Windows Hello for Business auch dann zur Verfügung stellen, wenn kein TPM verfügbar ist.|
|unlockWithBiometricsEnabled|Boolean|Steuert die Verwendung von biometrischen Gesten wie Gesicht und Fingerabdruck als Alternative zur Windows Hello for Business-PIN.  Wenn dieser Wert auf false festgelegt ist, sind biometrische Gesten nicht zulässig. Benutzer müssen bei Fehlern weiterhin eine PIN als Sicherung konfigurieren.|
|useCertificatesForOnPremisesAuthEnabled|Boolescher Wert|Boolescher Wert, der es Windows Hello for Business ermöglicht, Zertifikate zur Authentifizierung lokaler Ressourcen zu verwenden.|
|windowsHelloForBusinessBlocked|Boolescher Wert|Boolescher Wert, der Windows Hello for Business als Methode für die Anmeldung an Windows blockiert.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Sammlung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
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
  "useSecurityKeyForSignin": true,
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




