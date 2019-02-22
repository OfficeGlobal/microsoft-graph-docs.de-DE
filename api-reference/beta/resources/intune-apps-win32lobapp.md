---
title: win32LobApp-Ressourcentyp
description: Enthält Eigenschaften und geerbte Eigenschaften für Win32-apps.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c272f9b74e099d9a5112ab558a75596763a33b1b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145024"
---
# <a name="win32lobapp-resource-type"></a>win32LobApp-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften und geerbte Eigenschaften für Win32-apps.


Erbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Win32LobApps aufListen](../api/intune-apps-win32lobapp-list.md)|[win32LobApp](../resources/intune-apps-win32lobapp.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [win32LobApp](../resources/intune-apps-win32lobapp.md) -Objekte.|
|[Win32LobApp abrufen](../api/intune-apps-win32lobapp-get.md)|[win32LobApp](../resources/intune-apps-win32lobapp.md)|Lesen von Eigenschaften und Beziehungen des [win32LobApp](../resources/intune-apps-win32lobapp.md) -Objekts.|
|[Win32LobApp erstellen](../api/intune-apps-win32lobapp-create.md)|[win32LobApp](../resources/intune-apps-win32lobapp.md)|Erstellen eines neuen [win32LobApp](../resources/intune-apps-win32lobapp.md) -Objekts.|
|[Win32LobApp löschen](../api/intune-apps-win32lobapp-delete.md)|Keine|Löscht eine [win32LobApp](../resources/intune-apps-win32lobapp.md).|
|[Win32LobApp aktualisieren](../api/intune-apps-win32lobapp-update.md)|[win32LobApp](../resources/intune-apps-win32lobapp.md)|Aktualisieren der Eigenschaften eines [win32LobApp](../resources/intune-apps-win32lobapp.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|displayName|Zeichenfolge|Der vom Administrator bereitgestellte oder importierte Titel der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|description|String|Beschreibung der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|publisher|Zeichenfolge|Der Herausgeber der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|isFeatured|Boolescher Wert|Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|privacyInformationUrl|String|URL zur Datenschutzerklärung. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|informationUrl|Zeichenfolge|URL zur Seite mit weiteren Informationen. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|owner|Zeichenfolge|Der Besitzer der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|developer|Zeichenfolge|Der Entwickler der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|notes|Zeichenfolge|Hinweise zur App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|uploadState|Int32|Der Uploadstatus. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Der Veröffentlichungsstatus der App. Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde. Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt. Mögliche Werte sind: `notPublished`, `processing` und `published`.|
|isAssigned|Boolean|Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|Rolescopetagids zur|String collection|Liste der bereichstag-IDs für diese Mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|committedContentVersion|Zeichenfolge|Die interne zugesicherte Inhaltsversion. Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|fileName|String|Name der Hauptdatei der Branchenanwendung. Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|size|Int64|Gesamtgröße einschließlich aller hochgeladenen Dateien. Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|InstallCommandLine:|Zeichenfolge|Die Befehlszeile zum Installieren dieser APP|
|uninstallCommandLine|Zeichenfolge|Die Befehlszeile zum Deinstallieren dieser APP|
|applicableArchitectures|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|Die Windows-Architekturen, für die diese App ausgeführt werden kann. Mögliche Werte sind: `none`, `x86`, `x64`, `arm`, `neutral` und `arm64`.|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-apps-windowsminimumoperatingsystem.md)|Der Wert für die Mindestversion des verwendbaren Betriebssystems.|
|minimumFreeDiskSpaceInMB|Int32|Der Wert für den minimalen freien Speicherplatz, der erforderlich ist, um diese APP zu installieren.|
|minimumMemoryInMB|Int32|Der Wert für den minimalen physischen Arbeitsspeicher, der für die Installation dieser APP erforderlich ist.|
|minimumNumberOfProcessors|Int32|Der Wert für die Mindestanzahl von Prozessoren, die zum Installieren dieser APP erforderlich ist.|
|minimumCpuSpeedInMHz|Int32|Der Wert für die minimale CPU-Geschwindigkeit, die erforderlich ist, um diese APP zu installieren.|
|detectionRules|[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) -Sammlung|Die Erkennungsregeln zum Erkennen der Win32-Branchen-app.|
|installExperience|[win32LobAppInstallExperience](../resources/intune-apps-win32lobappinstallexperience.md)|Die Installationsumgebung für diese APP.|
|returnCodes|[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) -Sammlung|Die Rückgabecodes für das Verhalten nach der Installation.|
|msiInformation|[win32LobAppMsiInformation](../resources/intune-apps-win32lobappmsiinformation.md)|Die MSI-Details, wenn diese Win32-App eine MSI-APP ist.|
|setupFilePath|Zeichenfolge|Der relative Pfad der Setupdatei im verschlüsselten Win32LobApp-Paket.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Die Liste der Kategorien für diese App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Die Installationszusammenfassung für die mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Sammlung|Die Liste der Installationsstatus für diese Mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Sammlung|Die Liste der Installationsstatus für diese Mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|contentVersions|Sammlung von Objekten des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Liste der Versionen der App-Inhalte. Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.win32LobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "uploadState": 1024,
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "installCommandLine": "String",
  "uninstallCommandLine": "String",
  "applicableArchitectures": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "minimumFreeDiskSpaceInMB": 1024,
  "minimumMemoryInMB": 1024,
  "minimumNumberOfProcessors": 1024,
  "minimumCpuSpeedInMHz": 1024,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "String",
      "valueName": "String",
      "detectionType": "String",
      "operator": "String",
      "detectionValue": "String"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "String"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 1024,
      "type": "String"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "String",
    "productVersion": "String",
    "upgradeCode": "String",
    "requiresReboot": true,
    "packageType": "String",
    "productName": "String",
    "publisher": "String"
  },
  "setupFilePath": "String"
}
```




