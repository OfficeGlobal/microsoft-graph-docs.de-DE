---
title: Ressourcentyp osVersionCount
description: Anzahl der Geräte mit Malware für jede Version des Betriebssystems
ms.openlocfilehash: 7892761bd0dc20f09ab2deb47549aeb157e25644
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064232"
---
# <a name="osversioncount-resource-type"></a>Ressourcentyp osVersionCount

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Anzahl der Geräte mit Malware für jede Version des Betriebssystems
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|osVersion|String|Version des Betriebssystems|
|deviceCount|Int32|Anzahl der Geräte mit Malware für die Version des Betriebssystems|
|lastUpdateDateTime|DateTimeOffset|Der Zeitstempel der letzten Aktualisierung für die Anzahl der Geräte in UTC|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```





