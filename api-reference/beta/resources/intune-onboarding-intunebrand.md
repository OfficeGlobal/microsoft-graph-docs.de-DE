---
title: Ressourcentyp „intuneBrand“
description: „intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.
author: tfitzmac
ms.openlocfilehash: f59920d927e96f2c74e44670134e74a0db27dd7b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323541"
---
# <a name="intunebrand-resource-type"></a>Ressourcentyp „intuneBrand“

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

„intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|String|Unternehmensname/Organisationsname, der Endbenutzern angezeigt wird|
|contactITName|String|Name der für den IT-Support zuständigen Person/Organisation|
|contactITPhoneNumber|String|Telefonnummer der für den IT-Support zuständigen Person/Organisation|
|contactITEmailAddress|String|E-Mail-Adresse der für den IT-Support zuständigen Person/Organisation|
|contactITNotes|String|Textkommentare zu der für den IT-Support zuständigen Person/Organisation|
|privacyUrl|String|URL zur Datenschutzrichtlinie des Unternehmens/der Organisation|
|onlineSupportSiteUrl|String|URL zur IT-Helpdesk-Website des Unternehmens/der Organisation|
|onlineSupportSiteName|String|Anzeigename der IT-Helpdesk-Website des Unternehmens/der Organisation|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Primäres Farbdesign für die Unternehmensportal-Anwendungen und das Webportal|
|showLogo|Boolean|Boolescher Wert, der angibt, ob die vom Administrator bereitgestellten Logobilder angezeigt werden sollen|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Logobild, das in Unternehmensportal-Apps mit hellem Hintergrund hinter dem Logo angezeigt werden soll|
|darkBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Logobild, das in Unternehmensportal-Apps mit dunklem Hintergrund hinter dem Logo angezeigt werden soll|
|showNameNextToLogo|Boolean|Boolescher Wert, der angibt, ob der vom Administrator angegebene Anzeigename neben dem Logobild angezeigt werden soll|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Angepasste Bild im Unternehmen Portal-Angebotsseite|
|showDisplayNameNextToLogo|Boolean|Boolescher Wert, der angibt, ob der vom Administrator angegebene Anzeigename neben dem Logobild angezeigt werden soll|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
  "displayName": "String",
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "privacyUrl": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "darkBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showNameNextToLogo": true,
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showDisplayNameNextToLogo": true
}
```





