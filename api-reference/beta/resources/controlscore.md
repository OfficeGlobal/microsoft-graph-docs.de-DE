---
title: " Ressourcentyp controlScore"
description: Diese Ressource enthält einen Mandanten Score und eine Beschreibung für ein einzelnes Steuerelement.
localization_priority: Normal
ms.openlocfilehash: d8c2d73205f00a9dd5f2f28fcee3c33778bb3276
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891469"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="6ad56-103">Ressourcentyp controlScore</span><span class="sxs-lookup"><span data-stu-id="6ad56-103">controlScore resource type</span></span>

<span data-ttu-id="6ad56-104">Diese Ressource enthält einen Mandanten Score und eine Beschreibung für ein einzelnes Steuerelement.</span><span class="sxs-lookup"><span data-stu-id="6ad56-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="6ad56-105">Name</span><span class="sxs-lookup"><span data-stu-id="6ad56-105">Name</span></span> |<span data-ttu-id="6ad56-106">Typ</span><span class="sxs-lookup"><span data-stu-id="6ad56-106">Type</span></span> |<span data-ttu-id="6ad56-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ad56-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="6ad56-108">Steuerelementname</span><span class="sxs-lookup"><span data-stu-id="6ad56-108">controlName</span></span> |   <span data-ttu-id="6ad56-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6ad56-109">String</span></span>  |   <span data-ttu-id="6ad56-110">Eindeutiger Name des Steuerelements</span><span class="sxs-lookup"><span data-stu-id="6ad56-110">Control unique name</span></span> |
|   <span data-ttu-id="6ad56-111">score</span><span class="sxs-lookup"><span data-stu-id="6ad56-111">score</span></span>   |   <span data-ttu-id="6ad56-112">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="6ad56-112">Double</span></span>  |  <span data-ttu-id="6ad56-113">Mandanten erreicht Score für das Steuerelement (Dies hängt Tag je nach Mandant Vorgänge auf das Steuerelement).</span><span class="sxs-lookup"><span data-stu-id="6ad56-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="6ad56-114">controlCategory</span><span class="sxs-lookup"><span data-stu-id="6ad56-114">controlCategory</span></span> |   <span data-ttu-id="6ad56-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6ad56-115">String</span></span>  |  <span data-ttu-id="6ad56-116">Steuerelement-Aktionskategorie (Identität, Daten, Gerät, Apps, Infrastruktur).</span><span class="sxs-lookup"><span data-stu-id="6ad56-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="6ad56-117">description</span><span class="sxs-lookup"><span data-stu-id="6ad56-117">description</span></span> |   <span data-ttu-id="6ad56-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6ad56-118">String</span></span>  |  <span data-ttu-id="6ad56-119">Beschreibung des Steuerelements.</span><span class="sxs-lookup"><span data-stu-id="6ad56-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6ad56-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6ad56-120">JSON representation</span></span>

<span data-ttu-id="6ad56-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6ad56-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.controlScore"
}-->

```json
{
  "controlName": "String",
  "score": "String",
  "controlCategory": "String",
  "description": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "controlScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
