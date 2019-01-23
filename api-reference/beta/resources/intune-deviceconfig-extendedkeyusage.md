---
title: Ressourcentyp extendedKeyUsage
description: Benutzerdefinierte erweiterte Schlüsselverwendung definition
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ed825f44923d3fe86cc410397747b50a1f2c681
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425967"
---
# <a name="extendedkeyusage-resource-type"></a>Ressourcentyp extendedKeyUsage

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Benutzerdefinierte erweiterte Schlüsselverwendung definition

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|name|Zeichenfolge|Erweiterte Schlüsselverwendung Name|
|objectIdentifier|Zeichenfolge|Erweiterte Schlüsselverwendung Objektbezeichner|

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




