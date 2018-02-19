# <a name="windows10teamgeneralconfiguration-resource-type"></a>Ressourcentyp „windows10TeamGeneralConfiguration“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „windows10TeamGeneralConfiguration“ verfügbar gemacht werden.

Sie erbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „windows10TeamGeneralConfiguration“](../api/intune_deviceconfig_windows10teamgeneralconfiguration_list.md)|Sammlung von Objekten des Typs [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) auf.|
|[Abrufen von „windows10TeamGeneralConfiguration“](../api/intune_deviceconfig_windows10teamgeneralconfiguration_get.md)|[windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).|
|[Erstellen von „windows10TeamGeneralConfiguration“](../api/intune_deviceconfig_windows10teamgeneralconfiguration_create.md)|[windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md)|Erstellt neue Objekte des Typs [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).|
|[Löschen von „windows10TeamGeneralConfiguration“](../api/intune_deviceconfig_windows10teamgeneralconfiguration_delete.md)|Keiner|Löscht Objekte des Typs [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).|
|[Aktualisieren von „windows10TeamGeneralConfiguration“](../api/intune_deviceconfig_windows10teamgeneralconfiguration_update.md)|[windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md)|Aktualisiert die Eigenschaften von Objekten des Typs [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|azureOperationalInsightsBlockTelemetry|Boolean|Gibt an, ob Azure Operational Insights blockiert werden soll.|
|azureOperationalInsightsWorkspaceId|String|ID des Azure Operational Insights-Arbeitsbereichs|
|azureOperationalInsightsWorkspaceKey|String|Schlüssel des Azure Operational Insights-Arbeitsbereichs|
|connectAppBlockAutoLaunch|Boolean|Gibt an, ob die App „Verbinden“ automatisch gestartet werden soll, sobald eine Projektion initiiert wird.|
|maintenanceWindowBlocked|Boolean|Gibt an, ob ein Wartungsfenster für Geräteupdates festgelegt werden darf.|
|maintenanceWindowDurationInHours|Int32|Dauer des Wartungsfensters für Geräteupdates. Gültige Werte: 1 bis 5.|
|maintenanceWindowStartTime|TimeOfDay|Beginn des Wartungsfensters für Geräteupdates|
|miracastChannel|String|Kanal. Mögliche Werte sind: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne` und `oneHundredSixtyFive`.|
|miracastBlocked|Boolean|Gibt an, ob eine drahtlose Projektion erlaubt ist.|
|miracastRequirePin|Boolean|Gibt an, ob für eine drahtlose Projektion die Eingabe einer PIN erforderlich ist.|
|settingsBlockMyMeetingsAndFiles|Boolean|Gibt an, ob die Funktion „Meine Besprechungen und Dateien“ im Startmenü deaktiviert werden soll. In diesem Bereich werden die Office 365-Besprechungen und -Dateien des angemeldeten Benutzers angezeigt.|
|settingsBlockSessionResume|Boolean|Gibt an, ob Sitzungen nach einem Sitzungstimeout fortgeführt werden dürfen.|
|settingsBlockSigninSuggestions|Boolean|Gibt an, ob das Anmeldedialogfeld automatisch mit den Eingeladenen aus geplanten Besprechungen befüllt werden darf.|
|settingsDefaultVolume|Int32|Legt die Standardlautstärke für neue Sitzungen fest. Zulässige Werte sind 0 bis 100. Der Standardwert lautet 45. Gültige Werte: 0 bis 100.|
|settingsScreenTimeoutInMinutes|Int32|Gibt den Zeitraum in Minuten an, nach dem der Bildschirm des Hub-Systems abgeschaltet wird.|
|settingsSessionTimeoutInMinutes|Int32|Gibt den Zeitraum in Minuten an, nach dem es zu einem Sitzungstimeout kommt.|
|settingsSleepTimeoutInMinutes|Int32|Gibt den Zeitraum in Minuten an, nach dem das Hub-System in den Energiesparmodus geschaltet wird.|
|welcomeScreenBlockAutomaticWakeUp|Boolean|Gibt an, ob der Willkommensbildschirm automatisch angezeigt werden soll, sobald jemand den Raum betritt.|
|welcomeScreenBackgroundImageUrl|String|URL zum Hintergrundbild für den Willkommensbildschirm. Die URL muss das HTTPS-Protokoll verwenden und ein PNG-Bild zurückgeben.|
|welcomeScreenMeetingInformation|String|Die Informationen, die im Willkommensbildschirm angezeigt werden sollen. Mögliche Werte sind: `userDefined`, `showOrganizerAndTimeOnly` und `showOrganizerAndTimeAndSubject`.|

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
  "@odata.type": "microsoft.graph.windows10TeamGeneralConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "String",
  "azureOperationalInsightsWorkspaceKey": "String",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 1024,
  "maintenanceWindowStartTime": "String (time of day)",
  "miracastChannel": "String",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 1024,
  "settingsScreenTimeoutInMinutes": 1024,
  "settingsSessionTimeoutInMinutes": 1024,
  "settingsSleepTimeoutInMinutes": 1024,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "String",
  "welcomeScreenMeetingInformation": "String"
}
```



