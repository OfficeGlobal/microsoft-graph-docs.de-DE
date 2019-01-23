---
title: Ressourcentyp deviceManagementTroubleshootingErrorResource
description: -Objekt, der einen Link zu Informationen, die den Link zur Problembehandlung konnte der Azure-Verwaltungsportal oder eine Microsoft Doc sein.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5653801fb3e4575e642c012721b667f51e791cc1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430222"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a>Ressourcentyp deviceManagementTroubleshootingErrorResource

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

-Objekt, der einen Link zu Informationen, die den Link zur Problembehandlung konnte der Azure-Verwaltungsportal oder eine Microsoft Doc sein.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|text|String|Noch nicht dokumentiert|
|Link|Zeichenfolge|Den Link zur Webressource. Kann eine der folgenden Formatierungsprogramme enthalten: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorResource",
  "text": "String",
  "link": "String"
}
```




