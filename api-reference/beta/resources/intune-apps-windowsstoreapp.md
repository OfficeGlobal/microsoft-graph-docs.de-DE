---
title: windowsStoreApp-Ressourcentyp
description: Enthält Eigenschaften und geerbte Eigenschaften für Windows Store-Apps.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 753a756e342c20c08b5db5ace4dfc63c1facd559
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172128"
---
# <a name="windowsstoreapp-resource-type"></a>windowsStoreApp-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften und geerbte Eigenschaften für Windows Store-Apps.


Sie erbt von [mobileApp](../resources/intune-apps-mobileapp.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsStoreApps aufListen](../api/intune-apps-windowsstoreapp-list.md)|[windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) -Objekte.|
|[WindowsStoreApp abrufen](../api/intune-apps-windowsstoreapp-get.md)|[windowsStoreApp](../resources/intune-apps-windowsstoreapp.md)|Lesen von Eigenschaften und Beziehungen des [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) -Objekts.|
|[WindowsStoreApp erstellen](../api/intune-apps-windowsstoreapp-create.md)|[windowsStoreApp](../resources/intune-apps-windowsstoreapp.md)|Erstellen eines neuen [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) -Objekts.|
|[WindowsStoreApp löschen](../api/intune-apps-windowsstoreapp-delete.md)|Keine|Löscht eine [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md).|
|[WindowsStoreApp aktualisieren](../api/intune-apps-windowsstoreapp-update.md)|[windowsStoreApp](../resources/intune-apps-windowsstoreapp.md)|Aktualisieren der Eigenschaften eines [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) -Objekts.|

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
|appStoreUrl|Zeichenfolge|Die URL des Windows-APP-Speichers.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Die Liste der Kategorien für diese App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Die Installationszusammenfassung für die mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Sammlung|Die Liste der Installationsstatus für diese Mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Sammlung|Die Liste der Installationsstatus für diese Mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
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
  "appStoreUrl": "String"
}
```




