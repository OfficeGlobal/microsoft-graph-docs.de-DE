---
title: Ressourcentyp „mobileApp“
description: Eine abstrakte Klasse, die grundlegende Eigenschaften von mobilen Intune-Apps enthält
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c5b7af252c27f60a1b6dd78f7a69bc7a712541b9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938454"
---
# <a name="mobileapp-resource-type"></a>Ressourcentyp „mobileApp“

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine abstrakte Klasse, die grundlegende Eigenschaften von mobilen Intune-Apps enthält
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „mobileApp“](../api/intune-apps-mobileapp-list.md)|Sammlung von Objekten des Typs [mobileApp](../resources/intune-apps-mobileapp.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileApp](../resources/intune-apps-mobileapp.md) auf.|
|[Abrufen von „mobileApp“](../api/intune-apps-mobileapp-get.md)|[mobileApp](../resources/intune-apps-mobileapp.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [mobileApp](../resources/intune-apps-mobileapp.md).|
|[Aktion „assign“](../api/intune-apps-mobileapp-assign.md)|Keine|Noch nicht dokumentiert|
|[GetMobileAppCount-Funktion](../api/intune-apps-mobileapp-getmobileappcount.md)|Int64|Noch nicht dokumentiert|
|[GetTopMobileApps-Funktion](../api/intune-apps-mobileapp-gettopmobileapps.md)|[mobileApp](../resources/intune-apps-mobileapp.md)-Sammlung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|displayName|Zeichenfolge|Titel der App (vom Administrator bereitgestellt oder importiert)|
|description|Zeichenfolge|Beschreibung der App|
|publisher|Zeichenfolge|Herausgeber der App|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der App|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der App|
|isFeatured|Boolean|Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde|
|privacyInformationUrl|Zeichenfolge|URL zur Datenschutzerklärung|
|informationUrl|Zeichenfolge|URL zur Seite mit weiteren Informationen|
|owner|Zeichenfolge|Besitzer der App|
|developer|Zeichenfolge|Entwickler der App|
|notes|Zeichenfolge|Hinweise zur App.|
|uploadState|Int32|Der Upload-Zustand.|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Der Veröffentlichungsstatus der App. Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde. Mögliche Werte sind: `notPublished`, `processing` und `published`.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Liste der Kategorien, denen die App zugeordnet ist.|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App.|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Die Installationszusammenfassung für die mobile App.|
|deviceStatuses|[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Auflistung|Die Liste der Installationsstatus für diese mobile app.|
|userStatuses|[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Auflistung|Die Liste der Installationsstatus für diese mobile app.|

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
  "publishingState": "String"
}
```





