---
title: Ressourcentyp numberRange
description: Nummern Definition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 27393bdac6519078c2021e3484ae58ddf43216d9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416860"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="1cd6c-103">Ressourcentyp numberRange</span><span class="sxs-lookup"><span data-stu-id="1cd6c-103">numberRange resource type</span></span>

> <span data-ttu-id="1cd6c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1cd6c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1cd6c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1cd6c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1cd6c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1cd6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cd6c-107">Nummern Definition.</span><span class="sxs-lookup"><span data-stu-id="1cd6c-107">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="1cd6c-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1cd6c-108">Properties</span></span>
|<span data-ttu-id="1cd6c-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1cd6c-109">Property</span></span>|<span data-ttu-id="1cd6c-110">Typ</span><span class="sxs-lookup"><span data-stu-id="1cd6c-110">Type</span></span>|<span data-ttu-id="1cd6c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1cd6c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cd6c-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="1cd6c-112">lowerNumber</span></span>|<span data-ttu-id="1cd6c-113">Int32</span><span class="sxs-lookup"><span data-stu-id="1cd6c-113">Int32</span></span>|<span data-ttu-id="1cd6c-114">Niedrigere Zahl.</span><span class="sxs-lookup"><span data-stu-id="1cd6c-114">Lower number.</span></span>|
|<span data-ttu-id="1cd6c-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="1cd6c-115">upperNumber</span></span>|<span data-ttu-id="1cd6c-116">Int32</span><span class="sxs-lookup"><span data-stu-id="1cd6c-116">Int32</span></span>|<span data-ttu-id="1cd6c-117">Obergrenze.</span><span class="sxs-lookup"><span data-stu-id="1cd6c-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cd6c-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1cd6c-118">Relationships</span></span>
<span data-ttu-id="1cd6c-119">Keine</span><span class="sxs-lookup"><span data-stu-id="1cd6c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1cd6c-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1cd6c-120">JSON Representation</span></span>
<span data-ttu-id="1cd6c-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1cd6c-121">Here is a JSON representation of the resource.</span></span>
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




