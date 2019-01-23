---
title: Ressourcentyp deviceManagementTroubleshootingErrorDetails
description: Enthält detaillierte Informationen zu dem Fehler und seine Remediation-Objekt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9cdda64170afc739c23f1b258e5f2f1b31158662
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430010"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a>Ressourcentyp deviceManagementTroubleshootingErrorDetails

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Enthält detaillierte Informationen zu dem Fehler und seine Remediation-Objekt.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|context|Zeichenfolge|Noch nicht dokumentiert|
|failure|Zeichenfolge|Noch nicht dokumentiert|
|failureDetails|Zeichenfolge|Die detaillierte Beschreibung der Fehlerursache.|
|Wartung|Zeichenfolge|Die detaillierte Beschreibung der Vorgehensweise zur Behebung dieses Problems.|
|resources|[DeviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) -Auflistung|Enthält Links zu hilfreiche Dokumentation zu diesem Fehler.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorDetails",
  "context": "String",
  "failure": "String",
  "failureDetails": "String",
  "remediation": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
      "text": "String",
      "link": "String"
    }
  ]
}
```




