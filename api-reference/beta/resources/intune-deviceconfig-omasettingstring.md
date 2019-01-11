---
title: omaSettingString-Ressourcentyp
description: Zeichenfolgendefinition der OMA-Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 78dfbeaf89e25903efcacf65346c7dda70e53803
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874662"
---
# <a name="omasettingstring-resource-type"></a>omaSettingString-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Zeichenfolgendefinition der OMA-Einstellungen.

Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Anzeigename Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|description|Zeichenfolge|Beschreibung. Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|omaUri|Zeichenfolge|OMA Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|Wert|Zeichenfolge|Wert.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```





