---
title: Ressourcentyp „windowsMobileMSI“
description: Diese Ressource enthält die Eigenschaften und geerbten Eigenschaften einer branchenspezifischen Windows Mobile-MSI-App.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0a3ccd7ac2815e9279d27739a8eeeeb61c6cee31
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257701"
---
# <a name="windowsmobilemsi-resource-type"></a>Ressourcentyp „windowsMobileMSI“

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Diese Ressource enthält die Eigenschaften und geerbten Eigenschaften einer branchenspezifischen Windows Mobile-MSI-App.


Sie erbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „windowsMobileMSI“](../api/intune-apps-windowsmobilemsi-list.md)|Sammlung von Objekten des Typs [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) auf.|
|[Abrufen von „windowsMobileMSI“](../api/intune-apps-windowsmobilemsi-get.md)|[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).|
|[Erstellen von „windowsMobileMSI“](../api/intune-apps-windowsmobilemsi-create.md)|[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)|Erstellt neue Objekte des Typs [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).|
|[Löschen von „windowsMobileMSI“](../api/intune-apps-windowsmobilemsi-delete.md)|Keiner|Löscht Objekte des Typs [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).|
|[Aktualisieren von „windowsMobileMSI“](../api/intune-apps-windowsmobilemsi-update.md)|[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)|Aktualisiert die Eigenschaften von Objekten des Typs [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).|

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
|committedContentVersion|Zeichenfolge|Die interne zugesicherte Inhaltsversion. Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|fileName|Zeichenfolge|Name der Hauptdatei der Branchenanwendung. Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|size|Int64|Gesamtgröße einschließlich aller hochgeladenen Dateien. Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|commandLine|Zeichenfolge|Befehlszeile|
|productCode|Zeichenfolge|Produktcode|
|productVersion|Zeichenfolge|Produktversion der branchenspezifischen Windows Mobile-MSI-App.|
|ignoreVersionDetection|Boolean|Boolescher Wert, der steuert, ob nach der Installation der App auf einem Gerät die App-Version zur Erkennung der App verwendet werden soll. Setzen Sie diese Eigenschaft auf „true“ bei branchenspezifischen Windows Mobile-MSI-Apps, die sich selbstständig aktualisieren.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Die Liste der Kategorien für diese App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|contentVersions|Sammlung von Objekten des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Liste der Versionen der App-Inhalte. Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsMobileMSI"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "commandLine": "String",
  "productCode": "String",
  "productVersion": "String",
  "ignoreVersionDetection": true
}
```



