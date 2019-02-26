---
title: iosWebContentFilterSpecificWebsitesAccess-Ressourcentyp
description: Stellt einen iOS Web Content Filter-Einstellungstyp dar, der URL-Lesezeichen in den integrierten iOS-Browser installiert. Ein Beispielszenario befindet sich in der Unterrichtsumgebung, in der Lehrer möchten, dass die Schüler Websites über auf Ihren iOS-Geräten konfigurierte Browser-Lesezeichen navigieren und keinen Zugriff auf andere Websites haben.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c5ddd834ccd24d60e2696d49b64685d432f47196
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150309"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a>iosWebContentFilterSpecificWebsitesAccess-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt einen iOS Web Content Filter-Einstellungstyp dar, der URL-Lesezeichen in den integrierten iOS-Browser installiert. Ein Beispielszenario befindet sich in der Unterrichtsumgebung, in der Lehrer möchten, dass die Schüler Websites über auf Ihren iOS-Geräten konfigurierte Browser-Lesezeichen navigieren und keinen Zugriff auf andere Websites haben.


Erbt von [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|specificWebsitesOnly|[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) -Sammlung|URL-Lesezeichen, die in integrierten Browser und Benutzer installiert werden, dürfen nur über Lesezeichen auf Websites zugreifen. Diese Collection darf maximal 500 Elemente enthalten.|
|Website|[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) -Sammlung|URL-Lesezeichen, die in integrierten Browser und Benutzer installiert werden, dürfen nur über Lesezeichen auf Websites zugreifen. Diese Sammlung darf maximal 500 Elemente enthalten.|

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




