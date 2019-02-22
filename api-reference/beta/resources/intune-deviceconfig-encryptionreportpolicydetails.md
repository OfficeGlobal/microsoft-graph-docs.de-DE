---
title: encryptionReportPolicyDetails-Ressourcentyp
description: Richtlinien Details für den Verschlüsselungs Bericht
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9232acd2a155169385956b9d20b3011c963090a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177917"
---
# <a name="encryptionreportpolicydetails-resource-type"></a>encryptionReportPolicyDetails-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Richtlinien Details für den Verschlüsselungs Bericht

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|Richtlinien-Nr|Zeichenfolge|Richtlinien-ID für Verschlüsselungs Bericht|
|policyName|Zeichenfolge|Richtlinien Name für Verschlüsselungs Bericht|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.encryptionReportPolicyDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.encryptionReportPolicyDetails",
  "policyId": "String",
  "policyName": "String"
}
```




