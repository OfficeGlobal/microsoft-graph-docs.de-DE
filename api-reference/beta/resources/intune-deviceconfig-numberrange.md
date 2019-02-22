---
title: numberRange-Ressourcentyp
description: Nummernkreis Definition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 711206a256e17d6e10c7c54cf8a3dda4868db031
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166787"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="868d7-103">numberRange-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="868d7-103">numberRange resource type</span></span>

> <span data-ttu-id="868d7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="868d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="868d7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="868d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="868d7-106">Nummernkreis Definition.</span><span class="sxs-lookup"><span data-stu-id="868d7-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="868d7-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="868d7-107">Properties</span></span>
|<span data-ttu-id="868d7-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="868d7-108">Property</span></span>|<span data-ttu-id="868d7-109">Typ</span><span class="sxs-lookup"><span data-stu-id="868d7-109">Type</span></span>|<span data-ttu-id="868d7-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="868d7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="868d7-111">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="868d7-111">lowerNumber</span></span>|<span data-ttu-id="868d7-112">Int32</span><span class="sxs-lookup"><span data-stu-id="868d7-112">Int32</span></span>|<span data-ttu-id="868d7-113">Niedrigere Zahl.</span><span class="sxs-lookup"><span data-stu-id="868d7-113">Lower number.</span></span>|
|<span data-ttu-id="868d7-114">upperNumber</span><span class="sxs-lookup"><span data-stu-id="868d7-114">upperNumber</span></span>|<span data-ttu-id="868d7-115">Int32</span><span class="sxs-lookup"><span data-stu-id="868d7-115">Int32</span></span>|<span data-ttu-id="868d7-116">Obere Zahl.</span><span class="sxs-lookup"><span data-stu-id="868d7-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="868d7-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="868d7-117">Relationships</span></span>
<span data-ttu-id="868d7-118">Keine</span><span class="sxs-lookup"><span data-stu-id="868d7-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="868d7-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="868d7-119">JSON Representation</span></span>
<span data-ttu-id="868d7-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="868d7-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```




