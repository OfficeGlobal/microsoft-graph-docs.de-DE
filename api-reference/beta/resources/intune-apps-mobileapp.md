---
title: Ressourcentyp „mobileApp“
description: Eine abstrakte Klasse, die grundlegende Eigenschaften von mobilen Intune-Apps enthält
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94481902b7038ab9de9c845c938aac9bc9d409b9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154922"
---
# <a name="mobileapp-resource-type"></a>Ressourcentyp „mobileApp“

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Eine abstrakte Klasse, die grundlegende Eigenschaften von mobilen Intune-Apps enthält

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „mobileApp“](../api/intune-apps-mobileapp-list.md)|Sammlung von Objekten des Typs [mobileApp](../resources/intune-apps-mobileapp.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileApp](../resources/intune-apps-mobileapp.md) auf.|
|[Abrufen von „mobileApp“](../api/intune-apps-mobileapp-get.md)|[mobileApp](../resources/intune-apps-mobileapp.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [mobileApp](../resources/intune-apps-mobileapp.md).|
|[Aktion „assign“](../api/intune-apps-mobileapp-assign.md)|Keine|Noch nicht dokumentiert|
|[getMobileAppCount-Funktion](../api/intune-apps-mobileapp-getmobileappcount.md)|Int64|Noch nicht dokumentiert|
|[Gettopmobileappcount-Funktion](../api/intune-apps-mobileapp-gettopmobileapps.md)|[mobileApp](../resources/intune-apps-mobileapp.md)-Sammlung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität|
|displayName|Zeichenfolge|Titel der App (vom Administrator bereitgestellt oder importiert)|
|description|String|Beschreibung der App|
|publisher|Zeichenfolge|Herausgeber der App|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der App|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der App|
|isFeatured|Boolescher Wert|Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde|
|privacyInformationUrl|String|URL zur Datenschutzerklärung|
|informationUrl|Zeichenfolge|URL zur Seite mit weiteren Informationen|
|owner|Zeichenfolge|Besitzer der App|
|developer|Zeichenfolge|Entwickler der App|
|notes|Zeichenfolge|Hinweise zur App.|
|uploadState|Int32|Der Uploadstatus.|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Der Veröffentlichungsstatus der App. Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde. Mögliche Werte sind: `notPublished`, `processing` und `published`.|
|isAssigned|Boolean|Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.|
|Rolescopetagids zur|String collection|Liste der bereichstag-IDs für diese Mobile App.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Liste der Kategorien, denen die App zugeordnet ist.|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App.|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Die Installationszusammenfassung für die mobile App.|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Sammlung|Die Liste der Installationsstatus für diese Mobile App.|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Sammlung|Die Liste der Installationsstatus für diese Mobile App.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
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
  ]
}
```




