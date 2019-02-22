---
title: omaSettingFloatingPoint-Ressourcentyp
description: Gleitkommadefinition der OMA-Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4d1b1e4c2c02711d341f70bba28067489c3b817
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166808"
---
# <a name="omasettingfloatingpoint-resource-type"></a>omaSettingFloatingPoint-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Gleitkommadefinition der OMA-Einstellungen.


Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Anzeigename Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|description|String|Beschreibung. Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|omaUri|Zeichenfolge|OMA Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|Wert|Einzelner|Wert.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```




