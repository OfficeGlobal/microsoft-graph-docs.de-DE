---
title: Ressourcentyp embeddedSIMActivationCode
description: Der eingebettete SIM Aktivierungscode bereitgestellt vom Mobilfunkbetreiber.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 41976b92cfe6b6f695631dbd6c0d928c6ae99271
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878064"
---
# <a name="embeddedsimactivationcode-resource-type"></a>Ressourcentyp embeddedSIMActivationCode

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Der eingebettete SIM Aktivierungscode bereitgestellt vom Mobilfunkbetreiber.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|integratedCircuitCardIdentifier|Zeichenfolge|Chip Karte Bezeichner (ICCID) für diesen eingebettet SIM Aktivierungscode vom Mobilfunkbetreiber bereitgestellt.
Die Eingabe muss den folgenden regulären Ausdruck übereinstimmen: ' ^\[0-9\]{19}\[0-9\]?$ '.|
|matchingIdentifier|Zeichenfolge|Die MatchingIdentifier (MatchingID) gemäß den GSMA Zuordnung SGP.22 RSP technischen Spezifikationen Abschnitt 4.1.
Die Eingabe muss den folgenden regulären Ausdruck übereinstimmen: ' ^\[a-zA-Z0-9\-\]* $'.|
|smdpPlusServerAddress|Zeichenfolge|Der vollqualifizierte Domänenname des des SM-DP + Server wie in der technischen g/m2 Zuordnung SPG.22 RSP-Spezifikation angegeben.
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





