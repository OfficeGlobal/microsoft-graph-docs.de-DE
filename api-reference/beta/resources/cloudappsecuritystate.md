---
title: Ressourcentyp cloudAppSecurityState
description: Statusinformationen über die Cloudanwendung (DestinationServiceName, DestinationServiceIp) enthält.
ms.openlocfilehash: 915044c3084e3d9a9435d602ecc7ec809d2168f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062568"
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