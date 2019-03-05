---
title: operatingSystemVersionRange-Ressourcentyp
description: Version des Betriebssystems.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 521f7d0b0ec4ddab728ed3b95c27acf21695b0d3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148608"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="e3f82-103">operatingSystemVersionRange-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e3f82-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="e3f82-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3f82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3f82-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e3f82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3f82-106">Version des Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="e3f82-106">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="e3f82-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e3f82-107">Properties</span></span>
|<span data-ttu-id="e3f82-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e3f82-108">Property</span></span>|<span data-ttu-id="e3f82-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e3f82-109">Type</span></span>|<span data-ttu-id="e3f82-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3f82-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3f82-111">description</span><span class="sxs-lookup"><span data-stu-id="e3f82-111">description</span></span>|<span data-ttu-id="e3f82-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3f82-112">String</span></span>|<span data-ttu-id="e3f82-113">Die Beschreibung dieses Range-Beispiels (z. b. gültige 1702-Builds)</span><span class="sxs-lookup"><span data-stu-id="e3f82-113">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="e3f82-114">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="e3f82-114">lowestVersion</span></span>|<span data-ttu-id="e3f82-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3f82-115">String</span></span>|<span data-ttu-id="e3f82-116">Die niedrigste inklusive Version, die in diesem Range enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="e3f82-116">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="e3f82-117">highestVersion</span><span class="sxs-lookup"><span data-stu-id="e3f82-117">highestVersion</span></span>|<span data-ttu-id="e3f82-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3f82-118">String</span></span>|<span data-ttu-id="e3f82-119">Die höchste inklusive Version, die in diesem Range enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="e3f82-119">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3f82-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e3f82-120">Relationships</span></span>
<span data-ttu-id="e3f82-121">Keine</span><span class="sxs-lookup"><span data-stu-id="e3f82-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3f82-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e3f82-122">JSON Representation</span></span>
<span data-ttu-id="e3f82-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e3f82-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```




