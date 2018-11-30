---
title: Ressourcentyp vppTokenActionResult
description: Der Status der Aktion, die mit einem Apple Volume Purchase Program Token ausgeführt werden.
ms.openlocfilehash: d0cb9e21b04ccb8748d1f9e78f0a3e9dd465ce81
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065717"
---
# <a name="vpptokenactionresult-resource-type"></a>Ressourcentyp vppTokenActionResult

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Der Status der Aktion, die mit einem Apple Volume Purchase Program Token ausgeführt werden.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|actionName|Zeichenfolge|Name der Aktion|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Status der Aktion. Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.|
|startDateTime|DateTimeOffset|Zeitpunkt der Einleitung der Aktion|
|lastUpdatedDateTime|DateTimeOffset|Zeitpunkt der letzten Aktualisierung des Aktionszustands|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```





