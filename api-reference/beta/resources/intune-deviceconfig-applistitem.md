---
title: appListItem-Ressourcentyp
description: Stellt eine App in der Liste der verwalteten Anwendungen dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a7e005681917f0edffe00b33947d2bd2bd5b2ff5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172247"
---
# <a name="applistitem-resource-type"></a>appListItem-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt eine App in der Liste der verwalteten Anwendungen dar.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|name|Zeichenfolge|Anwendungsname|
|publisher|Zeichenfolge|Herausgeber der App|
|appStoreUrl|Zeichenfolge|Store-URL der Anwendung|
|appId|Zeichenfolge|Anwendungs- oder Paket-ID der Anwendung|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```




