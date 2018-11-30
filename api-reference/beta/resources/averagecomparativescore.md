---
title: " Ressourcentyp averageComparativeScore"
description: Diese Ressource enthält verschiedene unterschiedliche Faktoren, die von unterschiedlichen Bereichen (beispielsweise Durchschnitt von Branche vertikal, durchschnittliche vom Unternehmen Arbeitsplatz Größe usw.) und Steuerelement Kategorie (Identität, Daten, Gerät, Apps, Infrastruktur) basiert.
ms.openlocfilehash: 08e4ec60788b21476d8f1491ab5548c7a4ca2e01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059442"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="b0054-103">Ressourcentyp averageComparativeScore</span><span class="sxs-lookup"><span data-stu-id="b0054-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="b0054-104">Diese Ressource enthält verschiedene unterschiedliche Faktoren, die von unterschiedlichen Bereichen (beispielsweise Durchschnitt von Branche vertikal, durchschnittliche vom Unternehmen Arbeitsplatz Größe usw.) und Steuerelement Kategorie (Identität, Daten, Gerät, Apps, Infrastruktur) basiert.</span><span class="sxs-lookup"><span data-stu-id="b0054-104">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="b0054-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b0054-105">Property</span></span> |<span data-ttu-id="b0054-106">Typ</span><span class="sxs-lookup"><span data-stu-id="b0054-106">Type</span></span> |<span data-ttu-id="b0054-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0054-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="b0054-108">Basis</span><span class="sxs-lookup"><span data-stu-id="b0054-108">basis</span></span>   |   <span data-ttu-id="b0054-109">String</span><span class="sxs-lookup"><span data-stu-id="b0054-109">String</span></span>  |   <span data-ttu-id="b0054-110">Typ des Gültigkeitsbereichs (durch AllTenants TotalSeats, IndustryTypes).</span><span class="sxs-lookup"><span data-stu-id="b0054-110">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="b0054-111">averageScore</span><span class="sxs-lookup"><span data-stu-id="b0054-111">averageScore</span></span>    |   <span data-ttu-id="b0054-112">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="b0054-112">Double</span></span>  | <span data-ttu-id="b0054-113">Durchschnittliche Punktzahl innerhalb der angegebenen Basis.</span><span class="sxs-lookup"><span data-stu-id="b0054-113">Average score within specified basis.</span></span> |
|   <span data-ttu-id="b0054-114">deviceScore</span><span class="sxs-lookup"><span data-stu-id="b0054-114">deviceScore</span></span> |   <span data-ttu-id="b0054-115">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="b0054-115">Double</span></span>  | <span data-ttu-id="b0054-116">Durchschnittliche Punktzahl innerhalb der angegebenen Basis.</span><span class="sxs-lookup"><span data-stu-id="b0054-116">Average score within specified basis.</span></span> |
|   <span data-ttu-id="b0054-117">dataScore</span><span class="sxs-lookup"><span data-stu-id="b0054-117">dataScore</span></span>   |   <span data-ttu-id="b0054-118">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="b0054-118">Double</span></span>  | <span data-ttu-id="b0054-119">Durchschnittliche Punktzahl innerhalb der angegebenen Basis.</span><span class="sxs-lookup"><span data-stu-id="b0054-119">Average score within specified basis.</span></span> |
|   <span data-ttu-id="b0054-120">identityScore</span><span class="sxs-lookup"><span data-stu-id="b0054-120">identityScore</span></span>   |   <span data-ttu-id="b0054-121">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="b0054-121">Double</span></span>  | <span data-ttu-id="b0054-122">Durchschnittliche Punktzahl innerhalb der angegebenen Basis.</span><span class="sxs-lookup"><span data-stu-id="b0054-122">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b0054-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b0054-123">JSON representation</span></span>

<span data-ttu-id="b0054-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b0054-124">The following is a JSON representation of the resource.</span></span>

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
