---
title: iosDeviceType-Ressourcentyp
description: Enthält die Eigenschaften der möglichen iOS-Gerätetypen, auf denen die mobile App ausgeführt werden kann.
author: tfitzmac
ms.openlocfilehash: c9f691c2fdeb25bad54c105450c71dd7c65f30b1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342756"
---
# <a name="iosdevicetype-resource-type"></a>iosDeviceType-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält die Eigenschaften der möglichen iOS-Gerätetypen, auf denen die mobile App ausgeführt werden kann.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|iPad|Boolescher Wert|Gibt an, ob die App auf iPads ausgeführt werden soll.|
|iPhoneAndIPod|Boolescher Wert|Gibt an, ob die App auf iPhones und iPads ausgeführt werden soll.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceType",
  "iPad": true,
  "iPhoneAndIPod": true
}
```





