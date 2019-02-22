---
title: omaSettingBase64-Ressourcentyp
description: Base64-Definition der OMA-Einstellungen
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f6eae88e7158d5fd8d09caadda9fee6778182a9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166647"
---
# <a name="omasettingbase64-resource-type"></a>omaSettingBase64-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Base64-Definition der OMA-Einstellungen


Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Anzeigename Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|description|String|Beschreibung. Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).|
|omaUri|Zeichenfolge|OMA Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|fileName|Zeichenfolge|Die dem Dateinamen zugeordnete Werteigenschaft (*.cer | *. CRT | *. p7b | *. bin).|
|Wert|Zeichenfolge|Wert (Base64-codierte Zeichenfolge)|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```




