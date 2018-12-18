---
title: Ressourcentyp vppTokenLicenseSummary
description: Lizenz-Zusammenfassung der eine bestimmte app in einem Token.
author: tfitzmac
ms.openlocfilehash: 7847c6265ed526d50215567918698c7732adf947
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319978"
---
# <a name="vpptokenlicensesummary-resource-type"></a>Ressourcentyp vppTokenLicenseSummary

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Lizenz-Zusammenfassung der eine bestimmte app in einem Token.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|vppTokenId|String|Bezeichner des Tokens VPP.|
|appleId|String|Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist|
|organizationName|String|Die Organisation Apple Volume Purchase Programm Token zugeordnet.|
|availableLicenseCount|Int32|Die Anzahl der VPP Lizenzen zur Verfügung.|
|usedLicenseCount|Int32|Anzahl von VPP-Lizenzen, die aktuell verwendet werden.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenLicenseSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenLicenseSummary",
  "vppTokenId": "String",
  "appleId": "String",
  "organizationName": "String",
  "availableLicenseCount": 1024,
  "usedLicenseCount": 1024
}
```





