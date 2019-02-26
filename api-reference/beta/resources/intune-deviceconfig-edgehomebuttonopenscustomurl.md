---
title: edgeHomeButtonOpensCustomURL-Ressourcentyp
description: Schaltfläche "Start" anzeigen; beim Klicken auf die Schaltfläche "Startseite" wird eine bestimmte URL geladen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e83fd3dbb0961011584ef9d65e01c361ccf6a228
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143239"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a>edgeHomeButtonOpensCustomURL-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Schaltfläche "Start" anzeigen; beim Klicken auf die Schaltfläche "Startseite" wird eine bestimmte URL geladen.


Erbt von [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|homeButtonCustomURL|Zeichenfolge|Die zu ladende URL.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeHomeButtonOpensCustomURL"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeHomeButtonOpensCustomURL",
  "homeButtonCustomURL": "String"
}
```




