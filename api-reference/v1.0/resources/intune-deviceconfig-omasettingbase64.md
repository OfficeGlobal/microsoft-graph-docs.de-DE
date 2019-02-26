---
title: omaSettingBase64-Ressourcentyp
description: Base64-Definition der OMA-Einstellungen
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 678c6e78070a7aae185a041962083b7908ef1cc1
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258590"
---
# <a name="omasettingbase64-resource-type"></a>omaSettingBase64-Ressourcentyp

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



