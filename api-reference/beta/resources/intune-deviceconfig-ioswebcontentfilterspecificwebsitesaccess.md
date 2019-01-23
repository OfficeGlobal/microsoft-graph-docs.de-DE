---
title: Ressourcentyp iosWebContentFilterSpecificWebsitesAccess
description: Stellt eine iOS Web Content Filter Einstellungstyp, mit dem URL Textmarken in integrierten iOS-Browser installiert werden. Ein Beispielszenario ist im Kursraum, in dem Lehrer die Teilnehmer auf Websites durch Browser Lesezeichen in ihrer iOS-Geräte und keinen Zugriff auf andere Websites konfiguriert navigieren soll.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 964ade2d2b46755fbba2903c6e9607340f60aedf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424763"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a>Ressourcentyp iosWebContentFilterSpecificWebsitesAccess

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Stellt eine iOS Web Content Filter Einstellungstyp, mit dem URL Textmarken in integrierten iOS-Browser installiert werden. Ein Beispielszenario ist im Kursraum, in dem Lehrer die Teilnehmer auf Websites durch Browser Lesezeichen in ihrer iOS-Geräte und keinen Zugriff auf andere Websites konfiguriert navigieren soll.


Erbt vom [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|specificWebsitesOnly|[IosBookmark](../resources/intune-deviceconfig-iosbookmark.md) -Auflistung|URL Textmarken, die in integrierten Browser und Benutzer installiert werden darf nur durch Lesezeichen Websites zugreifen. Diese Collection darf maximal 500 Elemente enthalten.|
|websiteList|[IosBookmark](../resources/intune-deviceconfig-iosbookmark.md) -Auflistung|URL Textmarken, die in integrierten Browser und Benutzer installiert werden darf nur durch Lesezeichen Websites zugreifen. Diese Sammlung darf maximal 500 Elemente enthalten.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
  "specificWebsitesOnly": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ],
  "websiteList": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ]
}
```




