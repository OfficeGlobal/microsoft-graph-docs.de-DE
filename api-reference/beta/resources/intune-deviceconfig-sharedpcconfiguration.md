---
title: Ressourcentyp „sharedPCConfiguration“
description: In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „sharedPCConfiguration“ verfügbar gemacht werden.
ms.openlocfilehash: fec817184ed5027904b4afebcf867f45b2ac7808
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059778"
---
# <a name="sharedpcconfiguration-resource-type"></a>Ressourcentyp „sharedPCConfiguration“

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „sharedPCConfiguration“ verfügbar gemacht werden.

Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „sharedPCConfiguration“](../api/intune-deviceconfig-sharedpcconfiguration-list.md)|Sammlung von Objekten des Typs [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) auf.|
|[Abrufen von „sharedPCConfiguration“](../api/intune-deviceconfig-sharedpcconfiguration-get.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).|
|[Erstellen von „sharedPCConfiguration“](../api/intune-deviceconfig-sharedpcconfiguration-create.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)|Erstellt neue Objekte des Typs [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).|
|[Löschen von „sharedPCConfiguration“](../api/intune-deviceconfig-sharedpcconfiguration-delete.md)|Keiner|Löscht Objekte des Typs [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).|
|[Aktualisieren von „sharedPCConfiguration“](../api/intune-deviceconfig-sharedpcconfiguration-update.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)|Aktualisiert die Eigenschaften von Objekten des Typs [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).|

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
|accountManagerPolicy|[sharedPCAccountManagerPolicy](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|Gibt an, wie die Konten auf dem freigegebenen PC verwaltet werden sollen. Gilt nur, wenn für „disableAccountManager“ der Wert „false“ gesetzt ist.|
|allowedAccounts|[sharedPCAllowedAccountType](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|Gibt an, welche Typen von Konten auf einem freigegebenen PC verwendet werden dürfen. Mögliche Werte sind: `guest` und `domain`.|
|localStorage|[Aktivierung von Steuerelementen](../resources/intune-shared-enablement.md)|Gibt an, ob eine lokale Speicherung auf dem freigegebenen PC erlaubt ist. Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.|
|allowLocalStorage|Boolean|Gibt an, ob eine lokale Speicherung auf dem freigegebenen PC erlaubt ist.|
|setAccountManager|[Aktivierung von Steuerelementen](../resources/intune-shared-enablement.md)|Deaktiviert den Konto-Manager im Modus „Freigegebener PC“. Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.|
|disableAccountManager|Boolean|Deaktiviert den Konto-Manager im Modus „Freigegebener PC“.|
|setEduPolicies|[Aktivierung von Steuerelementen](../resources/intune-shared-enablement.md)|Gibt an, ob die standardmäßigen gemeinsamen PC Education-Umgebung Richtlinien aktiviert/deaktiviert/nicht konfiguriert werden soll. Ab Windows 10 RS2 wird diese Richtlinie auch dann angewendet, wenn „enabled“ nicht auf „true“ gesetzt ist. Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.|
|disableEduPolicies|Boolean|Gibt an, ob die standardmäßigen Schulungsumgebungsrichtlinien für freigegebene PCs deaktiviert werden sollen. Ab Windows 10 RS2 wird diese Richtlinie auch dann angewendet, wenn „enabled“ nicht auf „true“ gesetzt ist.|
|setPowerPolicies|[Aktivierung von Steuerelementen](../resources/intune-shared-enablement.md)|Gibt an, ob die standardmäßigen gemeinsamen PC Power Richtlinien aktiviert/deaktiviert sollte sein. Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.|
|disablePowerPolicies|Boolean|Gibt an, ob die standardmäßigen Energierichtlinien für freigegebene PCs deaktiviert werden sollen.|
|signInOnResume|[Aktivierung von Steuerelementen](../resources/intune-shared-enablement.md)|Gibt die Anforderung zum Signieren in immer das Gerät reaktiviert aus dem Standbymodus. Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.|
|disableSignInOnResume|Boolean|Legt fest, dass nicht bei jedem Aufwachen des Geräts aus dem Energiesparmodus eine erneute Anmeldung erforderlich ist.|
|enabled|Boolean|Aktiviert den Modus „Freigegebener PC“ und wendet die Richtlinien für freigegebene PCs an.|
|idleTimeBeforeSleepInSeconds|Int32|Gibt an, wie viele Sekunden sich der PC im Leerlauf befinden muss, bevor er in den Energiesparmodus geschaltet wird. Wird dieser Wert auf „0“ gesetzt, greift kein Timeout, das den PC in den Energiesparmodus versetzt.|
|kioskAppDisplayName|String|Gibt den Anzeigetext an, der dem Konto im Anmeldebildschirm angezeigt wird, über den die in „SetKioskAppUserModelId“ angegebene App gestartet wird. Gilt nur, wenn für „kioskAppUserModelId“ ein Wert festgelegt ist.|
|kioskAppUserModelId|String|Gibt die Anwendungsbenutzer-Modell-ID der App an, die über das Feature „Zugewiesener Zugriff“ genutzt werden darf.|
|maintenanceStartTime|TimeOfDay|Gibt den Beginn des täglichen Wartungszeitraums an.|

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
  "@odata.type": "microsoft.graph.sharedPCConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
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
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "String",
    "cacheAccountsAboveDiskFreePercentage": 1024,
    "inactiveThresholdDays": 1024,
    "removeAccountsBelowDiskFreePercentage": 1024
  },
  "allowedAccounts": "String",
  "localStorage": "String",
  "allowLocalStorage": true,
  "setAccountManager": "String",
  "disableAccountManager": true,
  "setEduPolicies": "String",
  "disableEduPolicies": true,
  "setPowerPolicies": "String",
  "disablePowerPolicies": true,
  "signInOnResume": "String",
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 1024,
  "kioskAppDisplayName": "String",
  "kioskAppUserModelId": "String",
  "maintenanceStartTime": "String (time of day)"
}
```





