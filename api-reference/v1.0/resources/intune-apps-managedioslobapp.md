---
title: managedIOSLobApp-Ressourcentyp
description: Enthält Eigenschaften und geerbte Eigenschaften für verwaltete branchenspezifische iOS-Apps.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e6b696d80f93b759111b2eb859c1d0a85502362
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255094"
---
# <a name="managedioslobapp-resource-type"></a>managedIOSLobApp-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften und geerbte Eigenschaften für verwaltete branchenspezifische iOS-Apps.


Sie erbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedIOSLobApps auflisten](../api/intune-apps-managedioslobapp-list.md)|[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekte.|
|[managedIOSLobApp abrufen](../api/intune-apps-managedioslobapp-get.md)|[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)|Lesen von Eigenschaften und Beziehungen des [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekts.|
|[managedIOSLobApp erstellen](../api/intune-apps-managedioslobapp-create.md)|[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)|Erstellen eines neuen [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekts.|
|[managedIOSLobApp löschen](../api/intune-apps-managedioslobapp-delete.md)|Keine|Löscht eine [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).|
|[managedIOSLobApp aktualisieren](../api/intune-apps-managedioslobapp-update.md)|[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)|Aktualisieren der Eigenschaften eines [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekts.|

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
|isFeatured|Boolean|Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|privacyInformationUrl|String|URL zur Datenschutzerklärung. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|informationUrl|Zeichenfolge|URL zur Seite mit weiteren Informationen. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|owner|Zeichenfolge|Der Besitzer der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|developer|Zeichenfolge|Der Entwickler der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|notes|Zeichenfolge|Hinweise zur App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Der Veröffentlichungsstatus der App. Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde. Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt. Mögliche Werte sind: `notPublished`, `processing` und `published`.|
|appAvailability|[managedAppAvailability](../resources/intune-apps-managedappavailability.md)|Die Verfügbarkeit der Anwendung. Von [ManagedApp](../resources/intune-apps-managedapp.md)geerbt. Mögliche Werte: `global`, `lineOfBusiness`.|
|version|String|Die Version der Anwendung. Geerbt von [managedApp](../resources/intune-apps-managedapp.md)|
|committedContentVersion|Zeichenfolge|Die interne zugesicherte Inhaltsversion. Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).|
|fileName|Zeichenfolge|Name der Hauptdatei der Branchenanwendung. Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).|
|size|Int64|Gesamtgröße einschließlich aller hochgeladenen Dateien. Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).|
|bundleId|Zeichenfolge|Identitätsname|
|applicableDeviceType|[iosDeviceType](../resources/intune-apps-iosdevicetype.md)|Die iOS-Architektur, für die diese App ausgeführt werden kann.|
|minimumSupportedOperatingSystem|[iosMinimumOperatingSystem](../resources/intune-apps-iosminimumoperatingsystem.md)|Der Wert für die Mindestversion des verwendbaren Betriebssystems.|
|expirationDateTime|DateTimeOffset|Das Ablaufdatum.|
|versionNumber|Zeichenfolge|Die Versionsnummer der verwalteten branchenspezifischen iOS-App.|
|buildNumber|Zeichenfolge|Die Buildnummer der verwalteten branchenspezifischen iOS-App.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Die Liste der Kategorien für diese App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|contentVersions|Sammlung von Objekten des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Liste der Versionen der App-Inhalte. Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedIOSLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "publishingState": "String",
  "appAvailability": "String",
  "version": "String",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "bundleId": "String",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "String (timestamp)",
  "versionNumber": "String",
  "buildNumber": "String"
}
```



