---
title: Ressourcentyp operatingSystemVersionRange
description: Betriebssystem Versionsbereich.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 56df6b53dc29247d3f718ad185152069a071a0f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875803"
---
# <a name="operatingsystemversionrange-resource-type"></a>Ressourcentyp operatingSystemVersionRange

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Betriebssystem Versionsbereich.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|description|String|Die Beschreibung dieses Bereichs (z. B. gültig 1702 Builds)|
|lowestVersion|String|Die niedrigste inklusive Version, die dieser Bereich enthält.|
|highestVersion|String|Die höchste inklusive Version, die dieser Bereich enthält.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```





