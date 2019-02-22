---
title: deviceManagementTroubleshootingErrorResource-Ressourcentyp
description: -Objekt, das einen Link zu Informationen zur Problembehandlung darstellt, kann die Verknüpfung zum Azure-Portal oder einem Microsoft-Dokument sein.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 25d97a6d085b9f1b7e0b1ab73361be3ac7ae74d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155559"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a>deviceManagementTroubleshootingErrorResource-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

-Objekt, das einen Link zu Informationen zur Problembehandlung darstellt, kann die Verknüpfung zum Azure-Portal oder einem Microsoft-Dokument sein.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|text|String|Noch nicht dokumentiert|
|Link|Zeichenfolge|Die Verknüpfung zur Webressource. Kann beliebige der folgenden Formatierungen enthalten: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}|

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




