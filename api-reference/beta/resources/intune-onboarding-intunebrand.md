---
title: Ressourcentyp „intuneBrand“
description: „intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3e899f418ea9214530ac3b70e493a15655ca873
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167382"
---
# <a name="intunebrand-resource-type"></a>Ressourcentyp „intuneBrand“

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

„intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Unternehmensname/Organisationsname, der Endbenutzern angezeigt wird|
|contactITName|Zeichenfolge|Name der für den IT-Support zuständigen Person/Organisation|
|contactITPhoneNumber|Zeichenfolge|Telefonnummer der für den IT-Support zuständigen Person/Organisation|
|contactITEmailAddress|Zeichenfolge|E-Mail-Adresse der für den IT-Support zuständigen Person/Organisation|
|contactITNotes|Zeichenfolge|Textkommentare zu der für den IT-Support zuständigen Person/Organisation|
|privacyUrl|Zeichenfolge|URL zur Datenschutzrichtlinie des Unternehmens/der Organisation|
|onlineSupportSiteUrl|Zeichenfolge|URL zur IT-Helpdesk-Website des Unternehmens/der Organisation|
|onlineSupportSiteName|String|Anzeigename der IT-Helpdesk-Website des Unternehmens/der Organisation|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Primäres Farbdesign für die Unternehmensportal-Anwendungen und das Webportal|
|showLogo|Boolean|Boolescher Wert, der angibt, ob die vom Administrator bereitgestellten Logobilder angezeigt werden sollen|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Logobild, das in Unternehmensportal-Apps mit hellem Hintergrund hinter dem Logo angezeigt werden soll|
|darkBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Logobild, das in Unternehmensportal-Apps mit dunklem Hintergrund hinter dem Logo angezeigt werden soll|
|showNameNextToLogo|Boolean|Boolescher Wert, der angibt, ob der vom Administrator angegebene Anzeigename neben dem Logobild angezeigt werden soll|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Angepasstes Bild, das auf der Zielseite der compnay-Portal App angezeigt wird|
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




