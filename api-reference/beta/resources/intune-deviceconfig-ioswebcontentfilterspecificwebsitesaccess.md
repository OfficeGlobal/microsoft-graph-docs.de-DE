---
title: Ressourcentyp iosWebContentFilterSpecificWebsitesAccess
description: Stellt eine iOS Web Content Filter Einstellungstyp, mit dem URL Textmarken in integrierten iOS-Browser installiert werden. Ein Beispielszenario ist im Kursraum, in dem Lehrer die Teilnehmer auf Websites durch Browser Lesezeichen in ihrer iOS-Geräte und keinen Zugriff auf andere Websites konfiguriert navigieren soll.
ms.openlocfilehash: c5e23905ab9e5b692500544161fc052dd606da5d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062437"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a>Ressourcentyp iosWebContentFilterSpecificWebsitesAccess

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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





