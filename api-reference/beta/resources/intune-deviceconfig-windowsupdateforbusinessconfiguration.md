---
title: Ressourcentyp „windowsUpdateForBusinessConfiguration“
description: Diese Ressource enthält die Windows Update for Business-Konfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d13a7f4a49e290f1f1ba6cc41b1071d6f4deb22d
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571543"
---
# <a name="windowsupdateforbusinessconfiguration-resource-type"></a>Ressourcentyp „windowsUpdateForBusinessConfiguration“

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Diese Ressource enthält die Windows Update for Business-Konfiguration.


Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „windowsUpdateForBusinessConfiguration“](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-list.md)|Sammlung von Objekten des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) auf.|
|[Abrufen von „windowsUpdateForBusinessConfiguration“](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-get.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).|
|[Erstellen von „windowsUpdateForBusinessConfiguration“](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-create.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)|Erstellt neue Objekte des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).|
|[Löschen von „windowsUpdateForBusinessConfiguration“](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-delete.md)|Keiner|Löscht Objekte des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).|
|[Aktualisieren von „windowsUpdateForBusinessConfiguration“](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-update.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)|Aktualisiert die Eigenschaften von Objekten des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).|
|[extendFeatureUpdatesPause-Aktion](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendfeatureupdatespause.md)|None|Extend-Feature-Updates halten für einen Windows Update for Business-Ring an.|
|[extendQualityUpdatesPause-Aktion](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendqualityupdatespause.md)|None|Extend Quality Updates Pause für ein Windows Update for Business-Ring.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolesch|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deliveryOptimizationMode|[windowsDeliveryOptimizationMode](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|Bereitstellungs OptimierungsModus. Mögliche Werte: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.|
|prereleaseFeatures|[prereleaseFeatures](../resources/intune-deviceconfig-prereleasefeatures.md)|Pre-Release-Funktionen. Mögliche Werte sind: `userDefined`, `settingsOnly`, `settingsAndExperimentations` und `notAllowed`.|
|automaticUpdateMode|[automaticUpdateMode](../resources/intune-deviceconfig-automaticupdatemode.md)|Modus für automatische Updates. Mögliche Werte: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.|
|microsoftUpdateServiceAllowed|Boolesch|Legt fest, dass der Microsoft Update Service zugelassen wird.|
|driversExcluded|Boolesch|Legt fest, dass Treiber von Windows-Updates ausgenommen werden.|
|installationSchedule|[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|Installationszeitplan|
|qualityUpdatesDeferralPeriodInDays|Int32|Legt fest, um wie viele Tage Qualitätsupdates zurückgestellt werden sollen.|
|featureUpdatesDeferralPeriodInDays|Int32|Legt fest, um wie viele Tage Funktionsupdates zurückgestellt werden sollen.|
|qualityUpdatesPaused|Boolesch|Setzt Qualitätsupdates aus.|
|featureUpdatesPaused|Boolean|Setzt Funktionsupdates aus.|
|qualityUpdatesPauseExpiryDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs der Aussetzung der Qualitätsupdates|
|featureUpdatesPauseExpiryDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs der Aussetzung der Funktionsupdates|
|businessReadyUpdatesOnly|[windowsUpdateType](../resources/intune-deviceconfig-windowsupdatetype.md)|Bestimmt, von welchen Zweigstellen die Aktualisierungen empfangen werden. Mögliche Werte sind: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow` und `windowsInsiderBuildRelease`.|
|skipChecksBeforeRestart|Boolesch|Alle Überprüfung vor Neustart überspringen: Akkustand = 40%, Benutzer Anwesenheit, Anzeige erforderlich, Präsentationsmodus, Vollbildmodus, Telefonanruf Status, Spielmodus usw. |
|updateWeeks|[windowsUpdateForBusinessUpdateWeeks](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|Updateinstallation für die Wochen des Monats geplant. Mögliche Werte sind: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek` und `everyWeek`.|
|qualityUpdatesPauseStartDate|Datum|Qualitäts Updates unterBrechen das Startdatum. Diese Eigenschaft ist schreibgeschützt.|
|featureUpdatesPauseStartDate|Datum|Feature-Updates unterBrechen Startdatum. Diese Eigenschaft ist schreibgeschützt.|
|featureUpdatesRollbackWindowInDays|Int32|Die Anzahl der Tage nach einer Funktions Aktualisierung, für die ein Rollback gültig ist.|
|qualityUpdatesWillBeRolledBack|Boolesch|Gibt an, ob bei der nächsten Geräteüberprüfung Rollback-Qualitäts Aktualisierungen vorgenommen werden.|
|featureUpdatesWillBeRolledBack|Boolesch|Gibt an, ob Feature-Updates bei der nächsten Geräteüberprüfung zurückgesetzt werden sollen.|
|qualityUpdatesRollbackStartDateTime|DateTimeOffset|Quality Updates Rollback Start DateTime|
|featureUpdatesRollbackStartDateTime|DateTimeOffset|Feature Updates Rollback Start DateTime|
|engagedRestartDeadlineInDays|Int32|Stichtag in Tagen vor automatischer Planung und Ausführung eines ausstehenden Neustarts außerhalb der aktiven Stunden, mit gültigem Bereich zwischen 2 und 30 Tagen|
|engagedRestartSnoozeScheduleInDays|Int32|Anzahl der Tage, die ein Benutzer zum erneuten Verfassen von Benachrichtigungen mit einem gültigen Gültigkeitszeitraum von 1 bis 3 Tagen aufgefordert werden kann.|
|engagedRestartTransitionScheduleInDays|Int32|Anzahl der Tage vor dem Übergang von automatischen Neustarts außerhalb der aktiven Stunden zu einem erneuten Neustart, die der Benutzer mit einem gültigen Bereich zwischen 0 und 30 Tagen planen muss.|
|autoRestartNotificationDismissal|[autoRestartNotificationDismissalMethod](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|Geben Sie die Methode an, mit der die erforderliche automatische Neustartbenachrichtigung geschlossen wird. Mögliche Werte sind: `notConfigured`, `automatic` und `user`.|
|scheduleRestartWarningInHours|Int32|Geben Sie den Zeitraum für Warnbenachrichtigungen für automatische Neustarts an. Unterstützte Werte: 2, 4, 8, 12 oder 24 (Stunden).|
|scheduleImminentRestartWarningInMinutes|Int32|Geben Sie den Zeitraum für den automatischen Neustart unmittelbar bevorstehender Warnbenachrichtigungen an. Unterstützte Werte: 15, 30 oder 60 (Minuten).|
|userPauseAccess|[Aktivierung](../resources/intune-shared-enablement.md)|Gibt an, ob der Zugriff von Endbenutzern auf Softwareupdates angehalten werden soll. Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.|
|userWindowsUpdateScanAccess|[Aktivierung](../resources/intune-shared-enablement.md)|Gibt an, ob der Benutzer Zugriff zum Überprüfen von Windows Update deaktiviert werden soll. Mögliche Werte sind: `notConfigured`, `enabled` und `disabled`.|
|updateNotificationLevel|[windowsUpdateNotificationDisplayOption](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|Gibt an, welche Windows Update-Benachrichtigungen angezeigt werden. Mögliche Werte sind: `notConfigured`, `defaultNotifications`, `restartWarningsOnly` und `disableAllNotifications`.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Sammlung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries|Sammlung von Objekten des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateForBusinessConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
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
  "deliveryOptimizationMode": "String",
  "prereleaseFeatures": "String",
  "automaticUpdateMode": "String",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "String",
    "scheduledInstallTime": "String (time of day)"
  },
  "qualityUpdatesDeferralPeriodInDays": 1024,
  "featureUpdatesDeferralPeriodInDays": 1024,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "String (timestamp)",
  "featureUpdatesPauseExpiryDateTime": "String (timestamp)",
  "businessReadyUpdatesOnly": "String",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "String",
  "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesRollbackWindowInDays": 1024,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "String (timestamp)",
  "featureUpdatesRollbackStartDateTime": "String (timestamp)",
  "engagedRestartDeadlineInDays": 1024,
  "engagedRestartSnoozeScheduleInDays": 1024,
  "engagedRestartTransitionScheduleInDays": 1024,
  "autoRestartNotificationDismissal": "String",
  "scheduleRestartWarningInHours": 1024,
  "scheduleImminentRestartWarningInMinutes": 1024,
  "userPauseAccess": "String",
  "userWindowsUpdateScanAccess": "String",
  "updateNotificationLevel": "String"
}
```




