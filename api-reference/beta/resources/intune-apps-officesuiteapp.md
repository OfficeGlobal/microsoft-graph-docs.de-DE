---
title: officeSuiteApp-Ressourcentyp
description: Enthält Eigenschaften und geerbte Eigenschaften für die Office365 Suite-app.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d7888edc73425c78090052222028e19f18ec8a1
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571375"
---
# <a name="officesuiteapp-resource-type"></a>officeSuiteApp-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften und geerbte Eigenschaften für die Office365 Suite-app.


Sie erbt von [mobileApp](../resources/intune-apps-mobileapp.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[OfficeSuiteApps aufListen](../api/intune-apps-officesuiteapp-list.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Objekte.|
|[OfficeSuiteApp abrufen](../api/intune-apps-officesuiteapp-get.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|Lesen von Eigenschaften und Beziehungen des [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Objekts.|
|[OfficeSuiteApp erstellen](../api/intune-apps-officesuiteapp-create.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|Erstellen eines neuen [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Objekts.|
|[OfficeSuiteApp löschen](../api/intune-apps-officesuiteapp-delete.md)|None|Löscht eine [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).|
|[OfficeSuiteApp aktualisieren](../api/intune-apps-officesuiteapp-update.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|Aktualisieren der Eigenschaften eines [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|displayName|Zeichenfolge|Der vom Administrator bereitgestellte oder importierte Titel der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|description|Zeichenfolge|Beschreibung der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|publisher|String|Der Herausgeber der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|isFeatured|Boolean|Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|privacyInformationUrl|String|URL zur Datenschutzerklärung Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|informationUrl|String|URL zur Seite mit weiteren Informationen. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|owner|String|Der Besitzer der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|developer|String|Der Entwickler der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|notes|String|Hinweise für die App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|uploadState|Int32|Der Uploadstatus. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Der Veröffentlichungsstatus für die App. Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde. Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt. Mögliche Werte sind: `notPublished`, `processing` und `published`.|
|isAssigned|Boolean|Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|Rolescopetagids zur|String collection|Liste der bereichstag-IDs für diese Mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|autoAcceptEula|Boolesch|Der Wert, der EULA automatisch auf dem Gerät des endBENUTZERs akzeptiert.|
|productIds|[officeProductId](../resources/intune-apps-officeproductid.md) -Sammlung|Die Produkt-IDs, die die SKU der Office365-Suite darstellen.|
|excludedApps|[excludedApps](../resources/intune-apps-excludedapps.md)|Die Eigenschaft zur Darstellung der apps, die von der ausgewählten Office365-Produkt-ID ausgeschlossen werden.|
|Eigenschaften usesharedcomputeractivation|Boolesch|Die Eigenschaft, die angibt, ob die Aktivierung gemeinsam genutzter Computer nicht für die Office365-App-Suite verwendet wird.|
|updateChannel|[officeUpdateChannel](../resources/intune-apps-officeupdatechannel.md)|Die Eigenschaft, die den Office365-Aktualisierungs Kanal darstellt. Mögliche Werte: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.|
|officePlatformArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|Die Eigenschaft, die die Version der Office365-App-Suite darstellt. Mögliche Werte sind: `none`, `x86`, `x64`, `arm`, `neutral` und `arm64`.|
|Localestoinstall wurden|String collection|Die Eigenschaft, die die Gebietsschemas darstellt, die bei der Installation der apps von Office365 installiert werden. Es verwendet Standard RFC 6033. Refhttps://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx|
|installProgressDisplayLevel|[officeSuiteInstallProgressDisplayLevel](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|So geben Sie die Anzeigeebene für die Setup-Benutzeroberfläche des InstallationsfortSchritts auf dem Gerät an. Mögliche Werte sind: `none` und `full`.|
|shouldUninstallOlderVersionsOfOffice|Boolesch|Die Eigenschaft, um zu bestimmen, ob eine vorhandene Office-MSI-Installation installiert werden soll, wenn eine Office365-App-Suite auf dem Gerät bereitgestellt wird.|
|targetVersion|String|Die Eigenschaft, die die spezifische Zielversion für die Office365-App-Suite darstellt, die auf den Geräten bereitgestellt bleiben soll.|
|updateVersion|String|Die Eigenschaft, die die Update Version darstellt, in der die spezifische Zielversion für die Office365-App-Suite verfügbar ist.|
|officeConfigurationXml|Binär|Die Eigenschaft, die die XML-Konfigurationsdatei darstellt, die für Office proPlus-apps angegeben werden kann. Vorrang vor allen anderen Eigenschaften. Wenn dieser Parameter vorhanden ist, wird die XML-Konfigurationsdatei zum Erstellen der APP verwendet.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Liste der Kategorien, denen die App zugeordnet ist. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Die Installationszusammenfassung für die mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Sammlung|Die Liste der Installationsstatus für diese Mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Sammlung|Die Liste der Installationsstatus für diese Mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeSuiteApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
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
  "autoAcceptEula": true,
  "productIds": [
    "String"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "teams": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "String",
  "officePlatformArchitecture": "String",
  "localesToInstall": [
    "String"
  ],
  "installProgressDisplayLevel": "String",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "String",
  "updateVersion": "String",
  "officeConfigurationXml": "binary"
}
```




