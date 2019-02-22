---
title: extendedKeyUsage-Ressourcentyp
description: Definition der benutzerdefinierten erweiterten Schlüsselverwendung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1487d217693135e26df99d4d72491abac4123ba7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173290"
---
# <a name="extendedkeyusage-resource-type"></a>extendedKeyUsage-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Definition der benutzerdefinierten erweiterten Schlüsselverwendung

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|name|Zeichenfolge|Name der erweiterten Schlüsselverwendung|
|objectIdentifier|Zeichenfolge|Bezeichner des erweiterten Schlüssel Verwendungs Objekts|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```




