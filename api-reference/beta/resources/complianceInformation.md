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
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="192ba-103">Ressourcentyp complianceInformation</span><span class="sxs-lookup"><span data-stu-id="192ba-103">complianceInformation resource type</span></span>

<span data-ttu-id="192ba-104">Enthält Compliance zugeordnete Daten secure Score-Steuerelement.</span><span class="sxs-lookup"><span data-stu-id="192ba-104">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="192ba-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="192ba-105">Property</span></span> |<span data-ttu-id="192ba-106">Typ</span><span class="sxs-lookup"><span data-stu-id="192ba-106">Type</span></span> |<span data-ttu-id="192ba-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="192ba-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="192ba-108">certificationName</span><span class="sxs-lookup"><span data-stu-id="192ba-108">certificationName</span></span> | <span data-ttu-id="192ba-109">string</span><span class="sxs-lookup"><span data-stu-id="192ba-109">string</span></span> | <span data-ttu-id="192ba-110">Compliance-Zertifizierung Namen (beispielsweise ISO 27018:2014, GDPR, FedRAMP, NIST 800 171)</span><span class="sxs-lookup"><span data-stu-id="192ba-110">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="192ba-111">certificationControls</span><span class="sxs-lookup"><span data-stu-id="192ba-111">certificationControls</span></span> | <span data-ttu-id="192ba-112">[CertificationControl](certificationcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="192ba-112">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="192ba-113">Auflistung der Steuerelemente Zertifizierung Zertifizierung zugeordnet</span><span class="sxs-lookup"><span data-stu-id="192ba-113">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="192ba-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="192ba-114">JSON representation</span></span>

<span data-ttu-id="192ba-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="192ba-115">The following is a JSON representation of the resource.</span></span>

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
