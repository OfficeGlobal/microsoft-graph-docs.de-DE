---
title: Ressourcentyp windowsPhone81AppX
description: Enthält Eigenschaften und geerbten Eigenschaften für Windows Phone 8.1 AppX-Line Of Business apps.
ms.openlocfilehash: 415595c4a527c76dc3c35b77b966762fbb7afa94
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064723"
---
# <a name="windowsphone81appx-resource-type"></a>Ressourcentyp windowsPhone81AppX

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften und geerbten Eigenschaften für Windows Phone 8.1 AppX-Line Of Business apps.

Erbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste windowsPhone81AppXs](../api/intune-apps-windowsphone81appx-list.md)|[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) -Auflistung|Listeneigenschaften und Beziehungen der [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) -Objekte.|
|[Abrufen von windowsPhone81AppX](../api/intune-apps-windowsphone81appx-get.md)|[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|Lesen Sie Eigenschaften und Beziehungen des [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) -Objekts.|
|[Erstellen von windowsPhone81AppX](../api/intune-apps-windowsphone81appx-create.md)|[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|Erstellen eines neuen [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) -Objekts.|
|[WindowsPhone81AppX löschen](../api/intune-apps-windowsphone81appx-delete.md)|Keines|Löscht eine [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).|
|[WindowsPhone81AppX aktualisieren](../api/intune-apps-windowsphone81appx-update.md)|[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|Aktualisieren Sie die Eigenschaften eines [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) -Objekts.|

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
|committedContentVersion|String|Die interne zugesicherte Inhaltsversion. Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|fileName|String|Name der Hauptdatei der Branchenanwendung. Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|size|Int64|Gesamtgröße einschließlich aller hochgeladenen Dateien. Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|applicableArchitectures|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|Die Windows-Architekturen, für die diese App ausgeführt werden kann. Mögliche Werte: `none`, `x86`, `x64`, `arm`, `neutral`.|
|identityName|String|Identitätsname|
|identityPublisherHash|String|Der Hash des Identitätsherausgebers.|
|identityResourceIdentifier|String|Der Identitätsressourcenbezeichner.|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-apps-windowsminimumoperatingsystem.md)|Der Wert für die Mindestversion des verwendbaren Betriebssystems.|
|phoneProductIdentifier|String|Die Produkt-ID des Telefons.|
|phonePublisherId|String|Die Telefon Publisher-Id.|
|identityVersion|String|Die Version der Identität|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Die Liste der Kategorien für diese App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Die Installationszusammenfassung für die mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|deviceStatuses|[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Auflistung|Die Liste der Installationsstatus für diese mobile app. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|userStatuses|[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Auflistung|Die Liste der Installationsstatus für diese mobile app. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|contentVersions|Sammlung von Objekten des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Liste der Versionen der App-Inhalte. Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPhone81AppX"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "applicableArchitectures": "String",
  "identityName": "String",
  "identityPublisherHash": "String",
  "identityResourceIdentifier": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "String",
  "phonePublisherId": "String",
  "identityVersion": "String"
}
```





