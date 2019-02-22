---
title: embeddedSIMActivationCode-Ressourcentyp
description: Der eingebettete SIM-Aktivierungscode, der vom Mobilfunkanbieter bereitgestellt wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 955dccb226332b297e30c4d40768f84936b04dbe
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145227"
---
# <a name="embeddedsimactivationcode-resource-type"></a>embeddedSIMActivationCode-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Der eingebettete SIM-Aktivierungscode, der vom Mobilfunkanbieter bereitgestellt wird.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|integratedCircuitCardIdentifier|Zeichenfolge|Der integrierte Leiterkarten Bezeichner (ICCID) für diesen eingebetteten SIM-Aktivierungscode, der vom Mobilfunkanbieter bereitgestellt wird.
die eingabe muss mit dem folgenden regulären ausdruck übereinstimmen:\['\]{19}\[^\]0-9 0-9 ? $ '.|
|matchingIdentifier|Zeichenfolge|Die MatchingIdentifier (übereinstimmende) gemäß der GSMA Association SGP. 22 RSP Technical Specification section 4,1.
Die Eingabe muss mit dem folgenden regulären Ausdruck übereinstimmen:\[' ^ a-zA-Z0\-\]-9 * $ '.|
|smdpPlusServerAddress|Zeichenfolge|Der vollqualifizierte Domänenname des SM-DP +-Servers gemäß der technischen Spezifikation des GSM-Verbandes SPG .22 RSP.
Die Eingabe muss mit dem folgenden regulären Ausdruck übereinstimmen: '\[^ (a-zA-Z0\]-9 +\[(-a-zA-Z0\]-9 +\.) *\[) + a-za\]{2,}-Z $ '.|

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




