---
title: Ressourcentyp unsupportedDeviceConfigurationDetail
description: Eine Beschreibung des warum ein Entity-Objekt nicht unterstützt wird.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6b82dcf28652cbe54a4932a641579101cb392639
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949773"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a>Ressourcentyp unsupportedDeviceConfigurationDetail

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine Beschreibung des warum ein Entity-Objekt nicht unterstützt wird.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|message|Zeichenfolge|Eine Nachricht erläutert, warum ein Entity-Objekt nicht unterstützt wird.|
|propertyName|Zeichenfolge|Wenn die Nachricht an eine bestimmte Eigenschaft in der ursprünglichen Entität, und klicken Sie dann auf den Namen dieser Eigenschaft verknüpft ist.|

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





