---
title: iosWebContentFilterAutoFilter-Ressourcentyp
description: Stellt einen iOS Web Content Filter-Einstellungstyp dar, der die automatische iOS-Filterfunktion ermöglicht und eine zusätzliche URL-Zugriffssteuerung ermöglicht. Wenn das iOS-Gerät ohne Eigenschaftswerte erstellt wird, wird der automatische Filter unabhängig davon aktiviert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74e281a4cbc08467730680b556e6e8026535ff3a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155664"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>iosWebContentFilterAutoFilter-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt einen iOS Web Content Filter-Einstellungstyp dar, der die automatische iOS-Filterfunktion ermöglicht und eine zusätzliche URL-Zugriffssteuerung ermöglicht. Wenn das iOS-Gerät ohne Eigenschaftswerte erstellt wird, wird der automatische Filter unabhängig davon aktiviert.


Erbt von [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|allowedUrls|String collection|Für den Zugriff zugelassene zusätzliche URLs|
|BlockierteURLs|String collection|Für Access blockierte zusätzliche URLs|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterAutoFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterAutoFilter",
  "allowedUrls": [
    "String"
  ],
  "blockedUrls": [
    "String"
  ]
}
```




