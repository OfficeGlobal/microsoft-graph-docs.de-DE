---
title: macOSLobApp-Ressourcentyp
description: Enthält Eigenschaften und geerbte Eigenschaften für die MacOS-Branchen-app.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49ee1f1ca3b9e9f05d2f9106dac4b9cf59309b9a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173451"
---
# <a name="macoslobapp-resource-type"></a>macOSLobApp-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften und geerbte Eigenschaften für die MacOS-Branchen-app.


Erbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[MacOSLobApps aufListen](../api/intune-apps-macoslobapp-list.md)|[macOSLobApp](../resources/intune-apps-macoslobapp.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [macOSLobApp](../resources/intune-apps-macoslobapp.md) -Objekte.|
|[MacOSLobApp abrufen](../api/intune-apps-macoslobapp-get.md)|[macOSLobApp](../resources/intune-apps-macoslobapp.md)|Lesen von Eigenschaften und Beziehungen des [macOSLobApp](../resources/intune-apps-macoslobapp.md) -Objekts.|
|[MacOSLobApp erstellen](../api/intune-apps-macoslobapp-create.md)|[macOSLobApp](../resources/intune-apps-macoslobapp.md)|Erstellen eines neuen [macOSLobApp](../resources/intune-apps-macoslobapp.md) -Objekts.|
|[MacOSLobApp löschen](../api/intune-apps-macoslobapp-delete.md)|Keine|Löscht eine [macOSLobApp](../resources/intune-apps-macoslobapp.md).|
|[MacOSLobApp aktualisieren](../api/intune-apps-macoslobapp-update.md)|[macOSLobApp](../resources/intune-apps-macoslobapp.md)|Aktualisieren der Eigenschaften eines [macOSLobApp](../resources/intune-apps-macoslobapp.md) -Objekts.|

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
|fileName|Zeichenfolge|Name der Hauptdatei der Branchenanwendung. Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|size|Int64|Gesamtgröße einschließlich aller hochgeladenen Dateien. Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|bundleId|Zeichenfolge|Die Bundle-ID.|
|minimumSupportedOperatingSystem|[macOSMinimumOperatingSystem](../resources/intune-apps-macosminimumoperatingsystem.md)|Wert, der angibt, welche Betriebssystemversion mindestens erforderlich ist|
|buildNumber|Zeichenfolge|Die Buildnummer der MacOS-app.|
|versionNumber|Zeichenfolge|Die Versionsnummer der MacOS-app.|
|childApps|[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) -Sammlung|Die APP-Liste in diesem Bundle-Paket|
|identityVersion|Zeichenfolge|Die Version der Identität|
|md5HashChunkSize|Int32|Die Chunkgröße für MD5-Hash|
|md5Hash|String collection|Die MD5-Hash-Codes|
|ignoreVersionDetection|Boolean|Boolescher Wert, der steuert, ob nach der Installation der App auf einem Gerät die App-Version zur Erkennung der App verwendet werden soll. Legen Sie diesen Wert auf true für macOS-Apps (Branchenanwendungen) fest, die eine Self-Update-Funktion verwenden.|

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
  "@odata.type": "microsoft.graph.macOSLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobApp",
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
  "bundleId": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true
  },
  "buildNumber": "String",
  "versionNumber": "String",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "String",
      "buildNumber": "String",
      "versionNumber": "String"
    }
  ],
  "identityVersion": "String",
  "md5HashChunkSize": 1024,
  "md5Hash": [
    "String"
  ],
  "ignoreVersionDetection": true
}
```




