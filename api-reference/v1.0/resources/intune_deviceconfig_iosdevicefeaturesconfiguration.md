# <a name="iosdevicefeaturesconfiguration-resource-type"></a>Ressourcentyp „iosDeviceFeaturesConfiguration“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Ressource repräsentiert das Konfigurationsprofil der Funktionen eines iOS-Geräts.

Sie erbt von [appleDeviceFeaturesConfigurationBase](../resources/intune_deviceconfig_appledevicefeaturesconfigurationbase.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „iosDeviceFeaturesConfiguration“](../api/intune_deviceconfig_iosdevicefeaturesconfiguration_list.md)|Sammlung von Objekten des Typs [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) auf.|
|[Abrufen von „iosDeviceFeaturesConfiguration“](../api/intune_deviceconfig_iosdevicefeaturesconfiguration_get.md)|[iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md).|
|[Erstellen von „iosDeviceFeaturesConfiguration“](../api/intune_deviceconfig_iosdevicefeaturesconfiguration_create.md)|[iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md)|Erstellt neue Objekte des Typs [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md).|
|[Löschen von „iosDeviceFeaturesConfiguration“](../api/intune_deviceconfig_iosdevicefeaturesconfiguration_delete.md)|Keiner|Löscht Objekte des Typs [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md).|
|[Aktualisieren von „iosDeviceFeaturesConfiguration“](../api/intune_deviceconfig_iosdevicefeaturesconfiguration_update.md)|[iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md)|Aktualisiert die Eigenschaften von Objekten des Typs [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Beschreibung|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|assetTagTemplate|Zeichenfolge|Bestandskennzeicheninformationen zum Gerät. Sie werden im Anmeldefenster und im Sperrbildschirm angezeigt.|
|lockScreenFootnote|Zeichenfolge|Fußnote, die im Anmeldefenster und im Sperrbildschirm angezeigt wird. Verfügbar ab iOS 9.3.1.|
|homeScreenDockIcons|Collection von Objekten des Typs [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)|Liste der Apps und Ordner, die im Home-Bildschirm-Dock angezeigt werden sollen. Diese Collection darf maximal 500 Elemente enthalten.|
|homeScreenPages|Collection von Objekten des Typs [iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md)|Liste der Seiten auf dem Home-Bildschirm. Diese Collection darf maximal 500 Elemente enthalten.|
|notificationSettings|Collection von Objekten des Typs [iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md)|Benachrichtigungseinstellungen für jede Bundle-ID. Gilt nur für Geräte im Betreuungsmodus (iOS 9.3 und höher). Diese Sammlung darf maximal 500 Elemente enthalten.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|Aufgaben|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.appleDeviceFeaturesConfigurationBase",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosDeviceFeaturesConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "assetTagTemplate": "String",
  "lockScreenFootnote": "String",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenItem",
      "displayName": "String",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "String",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "String",
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "String",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenItem",
          "displayName": "String",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "String",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "String",
                  "bundleID": "String"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "String",
      "appName": "String",
      "publisher": "String",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "String",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```








