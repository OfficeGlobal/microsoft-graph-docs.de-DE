---
title: " Ressourcentyp certificationControl"
description: Diese Ressource enthält Compliance Zertifizierung zugeordnete Daten secure Score-Steuerelement.
localization_priority: Normal
ms.openlocfilehash: 6f8269a85a8d3cb032f3e58457df95f4dd432c11
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810388"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="a5d61-103">Ressourcentyp certificationControl</span><span class="sxs-lookup"><span data-stu-id="a5d61-103">certificationControl resource type</span></span>

<span data-ttu-id="a5d61-104">Enthält Compliance Zertifizierung zugeordnete Daten secure Score-Steuerelement.</span><span class="sxs-lookup"><span data-stu-id="a5d61-104">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="a5d61-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a5d61-105">Property</span></span> |<span data-ttu-id="a5d61-106">Typ</span><span class="sxs-lookup"><span data-stu-id="a5d61-106">Type</span></span> |<span data-ttu-id="a5d61-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5d61-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="a5d61-108">name</span><span class="sxs-lookup"><span data-stu-id="a5d61-108">name</span></span> | <span data-ttu-id="a5d61-109">string</span><span class="sxs-lookup"><span data-stu-id="a5d61-109">string</span></span> | <span data-ttu-id="a5d61-110">Steuerelementname Zertifizierung (engl.)</span><span class="sxs-lookup"><span data-stu-id="a5d61-110">Certification control name</span></span> |
|<span data-ttu-id="a5d61-111">url</span><span class="sxs-lookup"><span data-stu-id="a5d61-111">url</span></span> | <span data-ttu-id="a5d61-112">string</span><span class="sxs-lookup"><span data-stu-id="a5d61-112">string</span></span> | <span data-ttu-id="a5d61-113">URL für den Microsoft-Dienst vertrauen Portal</span><span class="sxs-lookup"><span data-stu-id="a5d61-113">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a5d61-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a5d61-114">JSON representation</span></span>

<span data-ttu-id="a5d61-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a5d61-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificationControl"
}-->

```json
{
  "name": "String",
  "url": "Collection(microsoft.graph.certificationControl)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "certificationControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
