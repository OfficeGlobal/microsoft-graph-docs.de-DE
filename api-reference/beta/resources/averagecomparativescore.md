---
title: " Ressourcentyp averageComparativeScore"
description: Diese Ressource enthält verschiedene unterschiedliche Faktoren, die von unterschiedlichen Bereichen (beispielsweise Durchschnitt von Branche vertikal, durchschnittliche vom Unternehmen Arbeitsplatz Größe usw.) und Steuerelement Kategorie (Identität, Daten, Gerät, Apps, Infrastruktur) basiert.
localization_priority: Normal
ms.openlocfilehash: c32c1349edd70e80c1bf0fb12a36bd07e06ed39f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834594"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="22942-103">Ressourcentyp averageComparativeScore</span><span class="sxs-lookup"><span data-stu-id="22942-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="22942-104">Diese Ressource enthält verschiedene unterschiedliche Faktoren, die von unterschiedlichen Bereichen (beispielsweise Durchschnitt von Branche vertikal, durchschnittliche vom Unternehmen Arbeitsplatz Größe usw.) und Steuerelement Kategorie (Identität, Daten, Gerät, Apps, Infrastruktur) basiert.</span><span class="sxs-lookup"><span data-stu-id="22942-104">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="22942-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="22942-105">Property</span></span> |<span data-ttu-id="22942-106">Typ</span><span class="sxs-lookup"><span data-stu-id="22942-106">Type</span></span> |<span data-ttu-id="22942-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="22942-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="22942-108">Basis</span><span class="sxs-lookup"><span data-stu-id="22942-108">basis</span></span>   |   <span data-ttu-id="22942-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="22942-109">String</span></span>  |   <span data-ttu-id="22942-110">Typ des Gültigkeitsbereichs (durch AllTenants TotalSeats, IndustryTypes).</span><span class="sxs-lookup"><span data-stu-id="22942-110">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="22942-111">averageScore</span><span class="sxs-lookup"><span data-stu-id="22942-111">averageScore</span></span>    |   <span data-ttu-id="22942-112">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="22942-112">Double</span></span>  | <span data-ttu-id="22942-113">Durchschnittliche Punktzahl innerhalb der angegebenen Basis.</span><span class="sxs-lookup"><span data-stu-id="22942-113">Average score within specified basis.</span></span> |
|   <span data-ttu-id="22942-114">deviceScore</span><span class="sxs-lookup"><span data-stu-id="22942-114">deviceScore</span></span> |   <span data-ttu-id="22942-115">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="22942-115">Double</span></span>  | <span data-ttu-id="22942-116">Durchschnittliche Punktzahl innerhalb der angegebenen Basis.</span><span class="sxs-lookup"><span data-stu-id="22942-116">Average score within specified basis.</span></span> |
|   <span data-ttu-id="22942-117">dataScore</span><span class="sxs-lookup"><span data-stu-id="22942-117">dataScore</span></span>   |   <span data-ttu-id="22942-118">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="22942-118">Double</span></span>  | <span data-ttu-id="22942-119">Durchschnittliche Punktzahl innerhalb der angegebenen Basis.</span><span class="sxs-lookup"><span data-stu-id="22942-119">Average score within specified basis.</span></span> |
|   <span data-ttu-id="22942-120">identityScore</span><span class="sxs-lookup"><span data-stu-id="22942-120">identityScore</span></span>   |   <span data-ttu-id="22942-121">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="22942-121">Double</span></span>  | <span data-ttu-id="22942-122">Durchschnittliche Punktzahl innerhalb der angegebenen Basis.</span><span class="sxs-lookup"><span data-stu-id="22942-122">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="22942-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="22942-123">JSON representation</span></span>

<span data-ttu-id="22942-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="22942-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.averageComparativeScore"
}-->

```json
{
  "basis": "String",
  "averageScore": "Double",
  "deviceScore": "Double",
  "dataScore": "Double",
  "identityScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
