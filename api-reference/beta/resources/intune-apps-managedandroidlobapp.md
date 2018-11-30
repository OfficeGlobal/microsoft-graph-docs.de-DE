---
title: managedAndroidLobApp-Ressourcentyp
description: Enthält Eigenschaften und geerbte Eigenschaften für verwaltete branchenspezifische Android-Apps.
ms.openlocfilehash: d97826ed17316ce25603ebc9af2c07588830c7fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062022"
---
# <a name="managedandroidlobapp-resource-type"></a>managedAndroidLobApp-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften und geerbte Eigenschaften für verwaltete branchenspezifische Android-Apps.

Sie erbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedAndroidLobApps auflisten](../api/intune-apps-managedandroidlobapp-list.md)|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekte.|
|[managedAndroidLobApp abrufen](../api/intune-apps-managedandroidlobapp-get.md)|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)|Lesen von Eigenschaften und Beziehungen des [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts.|
|[managedAndroidLobApp erstellen](../api/intune-apps-managedandroidlobapp-create.md)|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)|Erstellen eines neuen [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts.|
|[managedAndroidLobApp löschen](../api/intune-apps-managedandroidlobapp-delete.md)|Keine|Löscht eine [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).|
|[managedAndroidLobApp aktualisieren](../api/intune-apps-managedandroidlobapp-update.md)|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)|Aktualisieren der Eigenschaften eines [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|displayName|String|Der vom Administrator bereitgestellte oder importierte Titel der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|description|String|Beschreibung der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|publisher|String|Der Herausgeber der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|isFeatured|Boolescher Wert|Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|privacyInformationUrl|String|URL zur Datenschutzerklärung. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|informationUrl|String|URL zur Seite mit weiteren Informationen. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|owner|String|Der Besitzer der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|developer|String|Der Entwickler der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|notes|String|Hinweise zur App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|uploadState|Int32|Der Upload-Zustand. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Der Veröffentlichungsstatus der App. Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde. Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md). Mögliche Werte sind: `notPublished`, `processing` und `published`.|
|appAvailability|[managedAppAvailability](../resources/intune-apps-managedappavailability.md)|Die Verfügbarkeit der Anwendung. Geerbt von [ManagedApp](../resources/intune-apps-managedapp.md). Mögliche Werte: `global`, `lineOfBusiness`.|
|version|String|Die Version der Anwendung. Geerbt von [managedApp](../resources/intune-apps-managedapp.md)|
|committedContentVersion|String|Die interne zugesicherte Inhaltsversion. Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).|
|fileName|String|Name der Hauptdatei der Branchenanwendung. Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).|
|size|Int64|Gesamtgröße einschließlich aller hochgeladenen Dateien. Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).|
|packageId|String|Bezeichner des Pakets|
|identityName|String|Identitätsname|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune-apps-androidminimumoperatingsystem.md)|Der Wert für die Mindestversion des verwendbaren Betriebssystems.|
|versionName|String|Der Versionsname der verwalteten branchenspezifischen Android-App.|
|versionCode|String|Der Codename der verwalteten branchenspezifischen Android-App.|
|identityVersion|String|Die Version der Identität|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Die Liste der Kategorien für diese App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Die Installationszusammenfassung für die mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|deviceStatuses|[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Auflistung|Die Liste der Installationsstatus für diese mobile app. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|userStatuses|[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Auflistung|Die Liste der Installationsstatus für diese mobile app. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|contentVersions|Sammlung von Objekten des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Liste der Versionen der App-Inhalte. Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAndroidLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "appAvailability": "String",
  "version": "String",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "packageId": "String",
  "identityName": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "String",
  "versionCode": "String",
  "identityVersion": "String"
}
```





