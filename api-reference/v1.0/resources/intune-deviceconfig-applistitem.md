---
title: appListItem-Ressourcentyp
description: Stellt eine App in der Liste der verwalteten Anwendungen dar.
author: tfitzmac
ms.openlocfilehash: a7e33b986f95f610abff2c7b5321f48f3668e488
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323597"
---
# <a name="applistitem-resource-type"></a>appListItem-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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



