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
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="74b16-103">Ressourcentyp complianceInformation</span><span class="sxs-lookup"><span data-stu-id="74b16-103">complianceInformation resource type</span></span>

<span data-ttu-id="74b16-104">Enthält Compliance zugeordnete Daten secure Score-Steuerelement.</span><span class="sxs-lookup"><span data-stu-id="74b16-104">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="74b16-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="74b16-105">Property</span></span> |<span data-ttu-id="74b16-106">Typ</span><span class="sxs-lookup"><span data-stu-id="74b16-106">Type</span></span> |<span data-ttu-id="74b16-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74b16-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="74b16-108">certificationName</span><span class="sxs-lookup"><span data-stu-id="74b16-108">certificationName</span></span> | <span data-ttu-id="74b16-109">string</span><span class="sxs-lookup"><span data-stu-id="74b16-109">string</span></span> | <span data-ttu-id="74b16-110">Compliance-Zertifizierung Namen (beispielsweise ISO 27018:2014, GDPR, FedRAMP, NIST 800 171)</span><span class="sxs-lookup"><span data-stu-id="74b16-110">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="74b16-111">certificationControls</span><span class="sxs-lookup"><span data-stu-id="74b16-111">certificationControls</span></span> | <span data-ttu-id="74b16-112">[CertificationControl](certificationcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="74b16-112">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="74b16-113">Auflistung der Steuerelemente Zertifizierung Zertifizierung zugeordnet</span><span class="sxs-lookup"><span data-stu-id="74b16-113">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="74b16-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="74b16-114">JSON representation</span></span>

<span data-ttu-id="74b16-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="74b16-115">The following is a JSON representation of the resource.</span></span>

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
