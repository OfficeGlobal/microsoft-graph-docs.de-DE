---
title: Ressourcentyp unsupportedDeviceConfigurationDetail
description: Eine Beschreibung des warum ein Entity-Objekt nicht unterstützt wird.
author: tfitzmac
ms.openlocfilehash: 4cccf49366a803e5f964605a4dc4ba7f56707823
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344051"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a>Ressourcentyp unsupportedDeviceConfigurationDetail

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine Beschreibung des warum ein Entity-Objekt nicht unterstützt wird.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|message|String|Eine Nachricht erläutert, warum ein Entity-Objekt nicht unterstützt wird.|
|propertyName|String|Wenn die Nachricht an eine bestimmte Eigenschaft in der ursprünglichen Entität, und klicken Sie dann auf den Namen dieser Eigenschaft verknüpft ist.|

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





