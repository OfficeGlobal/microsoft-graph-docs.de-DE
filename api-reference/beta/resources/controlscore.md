---
title: " Ressourcentyp controlScore"
description: Diese Ressource enthält einen Mandanten Score und eine Beschreibung für ein einzelnes Steuerelement.
ms.openlocfilehash: 67059c1a7382416411709f02c609c90b20a673b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059474"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="63a98-103">Ressourcentyp controlScore</span><span class="sxs-lookup"><span data-stu-id="63a98-103">controlScore resource type</span></span>

<span data-ttu-id="63a98-104">Diese Ressource enthält einen Mandanten Score und eine Beschreibung für ein einzelnes Steuerelement.</span><span class="sxs-lookup"><span data-stu-id="63a98-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="63a98-105">Name</span><span class="sxs-lookup"><span data-stu-id="63a98-105">Name</span></span> |<span data-ttu-id="63a98-106">Typ</span><span class="sxs-lookup"><span data-stu-id="63a98-106">Type</span></span> |<span data-ttu-id="63a98-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63a98-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="63a98-108">Steuerelementname</span><span class="sxs-lookup"><span data-stu-id="63a98-108">controlName</span></span> |   <span data-ttu-id="63a98-109">String</span><span class="sxs-lookup"><span data-stu-id="63a98-109">String</span></span>  |   <span data-ttu-id="63a98-110">Eindeutiger Name des Steuerelements</span><span class="sxs-lookup"><span data-stu-id="63a98-110">Control unique name</span></span> |
|   <span data-ttu-id="63a98-111">score</span><span class="sxs-lookup"><span data-stu-id="63a98-111">score</span></span>   |   <span data-ttu-id="63a98-112">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="63a98-112">Double</span></span>  |  <span data-ttu-id="63a98-113">Mandanten erreicht Score für das Steuerelement (Dies hängt Tag je nach Mandant Vorgänge auf das Steuerelement).</span><span class="sxs-lookup"><span data-stu-id="63a98-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="63a98-114">controlCategory</span><span class="sxs-lookup"><span data-stu-id="63a98-114">controlCategory</span></span> |   <span data-ttu-id="63a98-115">String</span><span class="sxs-lookup"><span data-stu-id="63a98-115">String</span></span>  |  <span data-ttu-id="63a98-116">Steuerelement-Aktionskategorie (Identität, Daten, Gerät, Apps, Infrastruktur).</span><span class="sxs-lookup"><span data-stu-id="63a98-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="63a98-117">description</span><span class="sxs-lookup"><span data-stu-id="63a98-117">description</span></span> |   <span data-ttu-id="63a98-118">String</span><span class="sxs-lookup"><span data-stu-id="63a98-118">String</span></span>  |  <span data-ttu-id="63a98-119">Beschreibung des Steuerelements.</span><span class="sxs-lookup"><span data-stu-id="63a98-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="63a98-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="63a98-120">JSON representation</span></span>

<span data-ttu-id="63a98-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="63a98-121">The following is a JSON representation of the resource.</span></span>

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
