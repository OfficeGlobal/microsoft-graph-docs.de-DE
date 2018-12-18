---
title: edgeSearchEngine-Ressourcentyp
description: Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.
author: tfitzmac
ms.openlocfilehash: bbe5ba35c9d5832a1910414f99a4de4e9fa957e2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361229"
---
# <a name="edgesearchengine-resource-type"></a>edgeSearchEngine-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.

Erbt von [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|edgeSearchEngineType|[edgeSearchEngineType](../resources/intune-deviceconfig-edgesearchenginetype.md)|Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen. Mögliche Werte: `default`, `bing`.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```





