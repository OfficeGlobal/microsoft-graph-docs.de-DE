---
title: Ressourcentyp osVersionCount
description: Anzahl der Geräte mit Malware für jede Version des Betriebssystems
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 227e802de7226d653d68997268c9bf4eac4aa259
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864148"
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





