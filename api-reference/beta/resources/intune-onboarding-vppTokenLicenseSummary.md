---
title: Ressourcentyp vppTokenLicenseSummary
description: Lizenz-Zusammenfassung der eine bestimmte app in einem Token.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0766fd4da996b57032154be98bbc22fd8c8a4a5b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939959"
---
# <a name="vpptokenlicensesummary-resource-type"></a>Ressourcentyp vppTokenLicenseSummary

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Lizenz-Zusammenfassung der eine bestimmte app in einem Token.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|vppTokenId|Zeichenfolge|Bezeichner des Tokens VPP.|
|appleId|Zeichenfolge|Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist|
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





