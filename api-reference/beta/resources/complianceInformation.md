---
title: " Ressourcentyp complianceInformation"
description: Diese Ressource enthält Compliance zugeordnete Daten secure Score-Steuerelement.
ms.openlocfilehash: a32670c6d11d391834358b769ae938a67b3d8aad
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380959"
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
