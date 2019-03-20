---
title: windowsKioskConfiguration-Ressourcentyp
description: Diese Entität enthält Beschreibungen der deklarierten Methoden, Eigenschaften und Beziehungen, die von der Kiosk-Ressource verfügbar gemacht werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63b9269086aa97b6be543abcc201288c00eba456
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572516"
---
# <a name="windowskioskconfiguration-resource-type"></a>windowsKioskConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Diese Entität enthält Beschreibungen der deklarierten Methoden, Eigenschaften und Beziehungen, die von der Kiosk-Ressource verfügbar gemacht werden.


Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsKioskConfigurations aufListen](../api/intune-deviceconfig-windowskioskconfiguration-list.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) -Objekte.|
|[WindowsKioskConfiguration abrufen](../api/intune-deviceconfig-windowskioskconfiguration-get.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) -Objekts.|
|[WindowsKioskConfiguration erstellen](../api/intune-deviceconfig-windowskioskconfiguration-create.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)|Erstellen eines neuen [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) -Objekts.|
|[WindowsKioskConfiguration löschen](../api/intune-deviceconfig-windowskioskconfiguration-delete.md)|Keine|Löscht eine [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).|
|[WindowsKioskConfiguration aktualisieren](../api/intune-deviceconfig-windowskioskconfiguration-update.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)|Aktualisieren der Eigenschaften eines [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolesch|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|kioskProfiles|[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) -Sammlung|Mit dieser Richtlinieneinstellung können Sie eine Liste der Kiosk Profile für eine Kiosk Konfiguration definieren. Diese Auflistung kann maximal drei Elemente enthalten.|
|kioskBrowserDefaultUrl|Zeichenfolge|Geben Sie die Standard-URL an, zu der der Browser beim Start navigieren soll.|
|kioskBrowserEnableHomeButton|Boolesch|Aktivieren Sie die Schaltfläche Home des Kiosk Browsers. Standardmäßig ist die Schaltfläche Start deaktiviert.|
|kioskBrowserEnableNavigationButtons|Boolesch|Aktivieren Sie die Navigationsschaltflächen des Kiosk Browsers (Forward/Back). Standardmäßig sind die Navigationsschaltflächen deaktiviert.|
|kioskBrowserEnableEndSessionButton|Boolesch|Aktivieren Sie die Schaltfläche Endsitzung des Kiosk Browsers. Standardmäßig ist die Schaltfläche Sitzung beenden deaktiviert.|
|kioskBrowserRestartOnIdleTimeInMinutes|Int32|Geben Sie die Anzahl der Minuten an, die die Sitzung inaktiv ist, bis der Kiosk-Browser neu gestartet wird.  Gültige Werte sind 1-1440. Gültige Werte 1 bis 1440|
|kioskBrowserBlockedURLs|String collection|Angeben von URLs, zu denen die Kiosk-Browser nicht navigieren sollen|
|kioskBrowserBlockedUrlExceptions|String collection|Angeben von URLs, zu denen der Kiosk Browser navigieren darf|
|edgeKioskEnablePublicBrowsing|Boolesch|Aktivieren Sie das öffentliche Browsen im Kioskmodus für den Microsoft Edge-Browser. Der Standardwert ist false.|

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
  "@odata.type": "microsoft.graph.windowsKioskConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
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
  "kioskProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsKioskProfile",
      "profileId": "String",
      "profileName": "String",
      "appConfiguration": {
        "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
        "apps": [
          {
            "@odata.type": "microsoft.graph.windowsKioskUWPApp",
            "startLayoutTileSize": "String",
            "name": "String",
            "appType": "String",
            "autoLaunch": true,
            "appUserModelId": "String",
            "appId": "String",
            "containedAppId": "String"
          }
        ],
        "showTaskBar": true,
        "allowAccessToDownloadsFolder": true,
        "disallowDesktopApps": true,
        "startMenuLayoutXml": "binary"
      },
      "userAccountsConfiguration": [
        {
          "@odata.type": "microsoft.graph.windowsKioskVisitor"
        }
      ]
    }
  ],
  "kioskBrowserDefaultUrl": "String",
  "kioskBrowserEnableHomeButton": true,
  "kioskBrowserEnableNavigationButtons": true,
  "kioskBrowserEnableEndSessionButton": true,
  "kioskBrowserRestartOnIdleTimeInMinutes": 1024,
  "kioskBrowserBlockedURLs": [
    "String"
  ],
  "kioskBrowserBlockedUrlExceptions": [
    "String"
  ],
  "edgeKioskEnablePublicBrowsing": true
}
```




