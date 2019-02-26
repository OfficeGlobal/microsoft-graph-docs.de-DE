---
title: iosBookmark-Ressourcentyp
description: iOS-URL-Lesezeichen
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9de5d95cd14931da850ab9bdaf5c581fd17f09dc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174996"
---
# <a name="iosbookmark-resource-type"></a>iosBookmark-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

iOS-URL-Lesezeichen

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|url|Zeichenfolge|URL erlaubt Zugriff|
|bookmarkFolder|Zeichenfolge|Der Ordner, in dem die Textmarke in Safari hinzugefügt werden soll.|
|displayName|String|Der Anzeigename der Textmarke|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosBookmark"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosBookmark",
  "url": "String",
  "bookmarkFolder": "String",
  "displayName": "String"
}
```




