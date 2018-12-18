---
title: edgeSearchEngineCustom-Ressourcentyp
description: Ermöglicht es IT-Administratoren, eine benutzerdefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.
author: tfitzmac
ms.openlocfilehash: f648f41bafcbaa37c972500139ecc8d3e70113ca
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357974"
---
# <a name="edgesearchenginecustom-resource-type"></a>edgeSearchEngineCustom-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Ermöglicht es IT-Administratoren, eine benutzerdefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.

Erbt von [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|edgeSearchEngineOpenSearchXmlUrl|Zeichenfolge|Verweist auf einen Https-Link mit der OpenSearch-XML-Datei, die mindestens den Kurznamen und die URL der Suchmaschine enthält.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineCustom",
  "edgeSearchEngineOpenSearchXmlUrl": "String"
}
```



