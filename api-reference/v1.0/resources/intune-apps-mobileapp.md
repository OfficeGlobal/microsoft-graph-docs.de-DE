---
title: Ressourcentyp „mobileApp“
description: Eine abstrakte Klasse, die grundlegende Eigenschaften von mobilen Intune-Apps enthält
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91167967a543ea4556c1704a2bba4ec9a10a4c3d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254065"
---
# <a name="mobileapp-resource-type"></a>Ressourcentyp „mobileApp“

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Eine abstrakte Klasse, die grundlegende Eigenschaften von mobilen Intune-Apps enthält

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „mobileApp“](../api/intune-apps-mobileapp-list.md)|Sammlung von Objekten des Typs [mobileApp](../resources/intune-apps-mobileapp.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileApp](../resources/intune-apps-mobileapp.md) auf.|
|[Abrufen von „mobileApp“](../api/intune-apps-mobileapp-get.md)|[mobileApp](../resources/intune-apps-mobileapp.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [mobileApp](../resources/intune-apps-mobileapp.md).|
|[Aktion „assign“](../api/intune-apps-mobileapp-assign.md)|Keine|Noch nicht dokumentiert|

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
|isFeatured|Boolean|Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde|
|privacyInformationUrl|String|URL zur Datenschutzerklärung|
|informationUrl|Zeichenfolge|URL zur Seite mit weiteren Informationen|
|owner|Zeichenfolge|Besitzer der App|
|developer|Zeichenfolge|Entwickler der App|
|notes|Zeichenfolge|Hinweise zur App|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Der Veröffentlichungsstatus der App. Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde. Mögliche Werte sind: `notPublished`, `processing` und `published`.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Liste der Kategorien, denen die App zugeordnet ist.|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung|Liste der Gruppenzuweisungen für die mobile App|

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
  "publishingState": "String"
}
```



