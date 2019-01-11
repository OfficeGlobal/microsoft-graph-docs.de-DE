---
title: Ressourcentyp cloudAppSecurityState
description: Statusinformationen über die Cloudanwendung (DestinationServiceName, DestinationServiceIp) enthält.
localization_priority: Normal
ms.openlocfilehash: ff76adf1d3879c3dac3f19ae122d82c9523d5193
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876804"
---
# <a name="cloudappsecuritystate-resource-type"></a>Ressourcentyp cloudAppSecurityState

Statusinformationen über die Cloudanwendung (DestinationServiceName, DestinationServiceIp) enthält.

## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|destinationServiceIp|String|Ziel-IP-Adresse der Verbindung mit der Cloud Anwendungsdienst.|
|destinationServiceName|String|Cloud-Anwendungsdienst/Name (zum Beispiel "Vertrieb", "Ablage" usw.).|
|riskScore|String|Provider-generiert/berechnet Risiko Score von der Anwendung/Clouddienst. Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
