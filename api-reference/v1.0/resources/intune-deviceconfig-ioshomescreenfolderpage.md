---
title: iosHomeScreenFolderPage-Ressourcentyp
description: Ein Ordner mit Apps auf der Startseite
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0417e7109d95c87083034fa9f7522c0f81dbfb99
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965852"
---
# <a name="ioshomescreenfolderpage-resource-type"></a>iosHomeScreenFolderPage-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Ein Ordner mit Apps auf der Startseite
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Name des Ordnerseite|
|Apps|[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)-Sammlung|Eine Liste der Apps, die auf einer Seite innerhalb eines Ordners angezeigt werden. Diese Sammlung kann bis zu 500 Elemente enthalten.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```



