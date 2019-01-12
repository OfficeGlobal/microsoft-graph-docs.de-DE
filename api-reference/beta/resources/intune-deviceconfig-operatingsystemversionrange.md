---
title: Ressourcentyp operatingSystemVersionRange
description: Betriebssystem Versionsbereich.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c0b81482ad4b48ad5fe59b1ec0109fcd3bf03f83
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918546"
---
# <a name="operatingsystemversionrange-resource-type"></a>Ressourcentyp operatingSystemVersionRange

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Betriebssystem Versionsbereich.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|description|Zeichenfolge|Die Beschreibung dieses Bereichs (z. B. gültig 1702 Builds)|
|lowestVersion|Zeichenfolge|Die niedrigste inklusive Version, die dieser Bereich enthält.|
|highestVersion|Zeichenfolge|Die höchste inklusive Version, die dieser Bereich enthält.|

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





