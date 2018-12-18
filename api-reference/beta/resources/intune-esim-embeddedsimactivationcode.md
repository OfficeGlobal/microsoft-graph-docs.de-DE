---
title: Ressourcentyp embeddedSIMActivationCode
description: Der eingebettete SIM Aktivierungscode bereitgestellt vom Mobilfunkbetreiber.
author: tfitzmac
ms.openlocfilehash: 4e768a4047b8ddc785b545d3b850128a8e44f256
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311788"
---
# <a name="embeddedsimactivationcode-resource-type"></a>Ressourcentyp embeddedSIMActivationCode

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Der eingebettete SIM Aktivierungscode bereitgestellt vom Mobilfunkbetreiber.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|integratedCircuitCardIdentifier|String|Chip Karte Bezeichner (ICCID) für diesen eingebettet SIM Aktivierungscode vom Mobilfunkbetreiber bereitgestellt.
Die Eingabe muss den folgenden regulären Ausdruck übereinstimmen: ' ^\[0-9\]{19}\[0-9\]?$ '.|
|matchingIdentifier|String|Die MatchingIdentifier (MatchingID) gemäß den GSMA Zuordnung SGP.22 RSP technischen Spezifikationen Abschnitt 4.1.
Die Eingabe muss den folgenden regulären Ausdruck übereinstimmen: ' ^\[a-zA-Z0-9\-\]* $'.|
|smdpPlusServerAddress|String|Der vollqualifizierte Domänenname des des SM-DP + Server wie in der technischen g/m2 Zuordnung SPG.22 RSP-Spezifikation angegeben.
Die Eingabe muss den folgenden regulären Ausdruck übereinstimmen: ' ^ (\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+) *\.) +\[a-zA-Z\]{2,}$'.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCode",
  "integratedCircuitCardIdentifier": "String",
  "matchingIdentifier": "String",
  "smdpPlusServerAddress": "String"
}
```





