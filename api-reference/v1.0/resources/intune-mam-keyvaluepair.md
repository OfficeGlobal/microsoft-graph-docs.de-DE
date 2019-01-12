---
title: keyValuePair-Ressourcentyp
description: Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: db3e24c1c14cb208be66b7a2b0364ad12b162956
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926442"
---
# <a name="keyvaluepair-resource-type"></a>keyValuePair-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|name|Zeichenfolge|Namen für dieses Schlüssel-Wert-Paar|
|Wert|Zeichenfolge|Wert für dieses Schlüssel-Wert-Paar|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```



