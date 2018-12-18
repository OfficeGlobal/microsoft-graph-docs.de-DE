---
title: Ressourcentyp operatingSystemVersionRange
description: Betriebssystem Versionsbereich.
author: tfitzmac
ms.openlocfilehash: b853e71b2d8f66d24122afb51cea97fc6a8f8d7e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331164"
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





