---
title: Ressourcentyp officeSuiteApp
description: Enthält Eigenschaften und geerbten Eigenschaften für die Office365-Suite-App.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 65ba9d39b2648ecf47e66c3b907eee50c57e906b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820559"
---
# <a name="officesuiteapp-resource-type"></a>Ressourcentyp officeSuiteApp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften und geerbten Eigenschaften für die Office365-Suite-App.

Sie erbt von [mobileApp](../resources/intune-apps-mobileapp.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste officeSuiteApps](../api/intune-apps-officesuiteapp-list.md)|[OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Auflistung|Listeneigenschaften und Beziehungen der [OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Objekte.|
|[Abrufen von officeSuiteApp](../api/intune-apps-officesuiteapp-get.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|Lesen Sie Eigenschaften und Beziehungen des [OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Objekts.|
|[Erstellen von officeSuiteApp](../api/intune-apps-officesuiteapp-create.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|Erstellen eines neuen [OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Objekts.|
|[OfficeSuiteApp löschen](../api/intune-apps-officesuiteapp-delete.md)|Keine|Löscht eine [OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md).|
|[OfficeSuiteApp aktualisieren](../api/intune-apps-officesuiteapp-update.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|Aktualisieren Sie die Eigenschaften eines [OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Objekts.|

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
|isFeatured|Boolean|Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|privacyInformationUrl|String|URL zur Datenschutzerklärung. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|informationUrl|String|URL zur Seite mit weiteren Informationen. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|owner|String|Der Besitzer der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|developer|String|Der Entwickler der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|notes|String|Hinweise zur App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|uploadState|Int32|Der Upload-Zustand. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Der Veröffentlichungsstatus der App. Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde. Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md). Mögliche Werte sind: `notPublished`, `processing` und `published`.|
|autoAcceptEula|Boolean|Der Wert, der automatisch auf den des Endbenutzers Gerät den Lizenzvertrag zu akzeptieren.|
|productIds|[OfficeProductId](../resources/intune-apps-officeproductid.md) -Auflistung|Die Produkt-Ids, die die Office365 Suite SKU darstellen.|
|excludedApps|[excludedApps](../resources/intune-apps-excludedapps.md)|Die Eigenschaft, um die apps darstellen, die von der ausgewählten Office365 Produkt-ID ausgeschlossen werden|
|useSharedComputerActivation|Boolean|Die Eigenschaft an, die darstellen, ob die Aktivierung gemeinsam genutzter Computer nicht für die app-Suite Office365 verwendet wird.|
|updateChannel|[officeUpdateChannel](../resources/intune-apps-officeupdatechannel.md)|Die Eigenschaft, die Update-Kanal Office365 darstellen. Mögliche Werte sind: `none`, `current`, `deferred`, `firstReleaseCurrent` und `firstReleaseDeferred`.|
|officePlatformArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|Die Eigenschaft, die Office365 app Suite Version darstellen. Mögliche Werte sind: `none`, `x86`, `x64`, `arm` und `neutral`.|
|localesToInstall|Collection von Objekten des Typs „String“|Die Eigenschaft, um die Gebietsschemas darstellen, die installiert werden Wenn apps aus Office365 installiert wird. Standard RFC 6033 verwendet. REF:https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx|
|installProgressDisplayLevel|[officeSuiteInstallProgressDisplayLevel](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|Sie können die Anzeigeebene für die Installation des Fortschritts Setup-Benutzeroberfläche auf dem Gerät angeben. Mögliche Werte sind: `none` und `full`.|
|shouldUninstallOlderVersionsOfOffice|Boolean|Die Eigenschaft zum bestimmen, ob das vorhandene Office MSI deinstallieren, wenn eine Office365 app-Suite auf dem Gerät bereitgestellt wird.|
|targetVersion|String|Die Eigenschaft, die bestimmte Zielversion für die app-Suite Office365 darstellen, die auf den Geräten bereitgestellten blieb werden sollte.|
|updateVersion|String|Die Eigenschaft, die Version darstellen, die bestimmten Zielversion für die app-Suite Office365 verfügbar ist.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Die Liste der Kategorien für diese App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Die Installationszusammenfassung für die mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|deviceStatuses|[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Auflistung|Die Liste der Installationsstatus für diese mobile app. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|userStatuses|[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Auflistung|Die Liste der Installationsstatus für diese mobile app. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|

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
  "updateVersion": "String"
}
```





