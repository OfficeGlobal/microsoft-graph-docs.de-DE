---
title: " Ressourcentyp complianceInformation"
description: Diese Ressource enthält Compliance zugeordnete Daten secure Score-Steuerelement.
localization_priority: Normal
ms.openlocfilehash: 7a3968e6e043d2019100870061c5e34b03b1b8bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820601"
---
#  <a name="complianceinformation-resource-type"></a>Ressourcentyp complianceInformation

Enthält Compliance zugeordnete Daten secure Score-Steuerelement.

|Eigenschaft |Typ |Beschreibung |
|:--|:--|:--|
|certificationName | string | Compliance-Zertifizierung Namen (beispielsweise ISO 27018:2014, GDPR, FedRAMP, NIST 800 171) |
|certificationControls | [CertificationControl](certificationcontrol.md) -Auflistung | Auflistung der Steuerelemente Zertifizierung Zertifizierung zugeordnet |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.complianceInformation"
}-->

```json
{
  "certificationName": "String",
  "certificationControls": "Collection(microsoft.graph.complianceInformation)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "complianceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
