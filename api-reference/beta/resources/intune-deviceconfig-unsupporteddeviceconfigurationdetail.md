---
title: unsupportedDeviceConfigurationDetail-Ressourcentyp
description: Eine Beschreibung, warum eine Entität nicht unterstützt wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6ebdb6eb91dd64c1605288cc0cb1260f8fe7440a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148468"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a>unsupportedDeviceConfigurationDetail-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Eine Beschreibung, warum eine Entität nicht unterstützt wird.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|message|Zeichenfolge|Eine Meldung, die erklärt, warum eine Entität nicht unterstützt wird.|
|propertyName|Zeichenfolge|Wenn die Nachricht mit einer bestimmten Eigenschaft in der ursprünglichen Entität verknüpft ist, dann der Name dieser Eigenschaft.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfigurationDetail",
  "message": "String",
  "propertyName": "String"
}
```




