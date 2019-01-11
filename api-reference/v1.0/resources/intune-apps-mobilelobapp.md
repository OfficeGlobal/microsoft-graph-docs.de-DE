---
title: mobileLobApp-Ressourcentyp
description: Eine abstrakte Basisklasse mit Eigenschaften für alle mobilen branchenspezifischen Apps.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4c36fbccf3549367cb0f6d58c5b50d6fc46a018a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860760"
---
# <a name="mobilelobapp-resource-type"></a>mobileLobApp-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine abstrakte Basisklasse mit Eigenschaften für alle mobilen branchenspezifischen Apps.

Sie erbt von [mobileApp](../resources/intune-apps-mobileapp.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[MobileLobApps auflisten](../api/intune-apps-mobilelobapp-list.md)|[mobileLobApp](../resources/intune-apps-mobilelobapp.md)-Sammlung|Listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileLobApp](../resources/intune-apps-mobilelobapp.md) auf.|
|[MobileLobApp abrufen](../api/intune-apps-mobilelobapp-get.md)|[mobileLobApp](../resources/intune-apps-mobilelobapp.md)|Liest die Eigenschaften und Beziehungen von Objekten des [mobileLobApp](../resources/intune-apps-mobilelobapp.md)-Objekts auf.|

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
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Der Veröffentlichungsstatus der App. Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde. Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md). Mögliche Werte sind: `notPublished`, `processing` und `published`.|
|committedContentVersion|String|Die interne zugesicherte Inhaltsversion.|
|fileName|String|Der Name der Hauptdatei der Branchenanwendung.|
|size|Int64|Die Gesamtgröße einschließlich aller hochgeladenen Dateien.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Die Liste der Kategorien für diese App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|contentVersions|Sammlung von Objekten des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Die Liste der Inhaltsversionen für diese App.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileLobApp",
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
  "size": 1024
}
```



