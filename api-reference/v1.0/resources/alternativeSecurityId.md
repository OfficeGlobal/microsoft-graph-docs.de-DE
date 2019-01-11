---
title: alternativeSecurityId-Ressourcentyp
description: Nur für internen Gebrauch.
localization_priority: Normal
ms.openlocfilehash: 23ef74085a4a3cc383f0854e9139c9a0b63e3d40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853802"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="fba17-103">alternativeSecurityId-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fba17-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="fba17-104">Nur für internen Gebrauch.</span><span class="sxs-lookup"><span data-stu-id="fba17-104">For internal use only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fba17-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fba17-105">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "type": 12345,
  "identityProvider": "string",
  "key": {"@odata.type": "Edm.Binary"}
}
```

## <a name="properties"></a><span data-ttu-id="fba17-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fba17-106">Properties</span></span>
| <span data-ttu-id="fba17-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fba17-107">Property</span></span>         | <span data-ttu-id="fba17-108">Typ</span><span class="sxs-lookup"><span data-stu-id="fba17-108">Type</span></span>       | <span data-ttu-id="fba17-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fba17-109">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="fba17-110">Typ</span><span class="sxs-lookup"><span data-stu-id="fba17-110">type</span></span>             | <span data-ttu-id="fba17-111">Int32</span><span class="sxs-lookup"><span data-stu-id="fba17-111">Int32</span></span>      | <span data-ttu-id="fba17-112">Nur zur internen Verwendung</span><span class="sxs-lookup"><span data-stu-id="fba17-112">For internal use only</span></span>
| <span data-ttu-id="fba17-113">identityProvider</span><span class="sxs-lookup"><span data-stu-id="fba17-113">identityProvider</span></span> | <span data-ttu-id="fba17-114">string</span><span class="sxs-lookup"><span data-stu-id="fba17-114">string</span></span>     | <span data-ttu-id="fba17-115">Nur zur internen Verwendung</span><span class="sxs-lookup"><span data-stu-id="fba17-115">For internal use only</span></span>
| <span data-ttu-id="fba17-116">Key</span><span class="sxs-lookup"><span data-stu-id="fba17-116">key</span></span>              | <span data-ttu-id="fba17-117">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="fba17-117">Edm.Binary</span></span> | <span data-ttu-id="fba17-118">Nur zur internen Verwendung</span><span class="sxs-lookup"><span data-stu-id="fba17-118">For internal use only</span></span>
