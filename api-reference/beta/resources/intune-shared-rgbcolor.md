---
title: rgbColor-Ressourcentyp
description: Farbe in RGB
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 505383227d1014f779cb558d43c18da29d3989aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395517"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="ac98a-103">rgbColor-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ac98a-103">rgbColor resource type</span></span>

> <span data-ttu-id="ac98a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ac98a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ac98a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ac98a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ac98a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ac98a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac98a-107">Farbe in RGB</span><span class="sxs-lookup"><span data-stu-id="ac98a-107">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="ac98a-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ac98a-108">Properties</span></span>
|<span data-ttu-id="ac98a-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ac98a-109">Property</span></span>|<span data-ttu-id="ac98a-110">Typ</span><span class="sxs-lookup"><span data-stu-id="ac98a-110">Type</span></span>|<span data-ttu-id="ac98a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac98a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac98a-112">r</span><span class="sxs-lookup"><span data-stu-id="ac98a-112">r</span></span>|<span data-ttu-id="ac98a-113">Byte</span><span class="sxs-lookup"><span data-stu-id="ac98a-113">Byte</span></span>|<span data-ttu-id="ac98a-114">Rotwert</span><span class="sxs-lookup"><span data-stu-id="ac98a-114">Red value</span></span>|
|<span data-ttu-id="ac98a-115">g</span><span class="sxs-lookup"><span data-stu-id="ac98a-115">g</span></span>|<span data-ttu-id="ac98a-116">Byte</span><span class="sxs-lookup"><span data-stu-id="ac98a-116">Byte</span></span>|<span data-ttu-id="ac98a-117">Grünwert</span><span class="sxs-lookup"><span data-stu-id="ac98a-117">Green value</span></span>|
|<span data-ttu-id="ac98a-118">b</span><span class="sxs-lookup"><span data-stu-id="ac98a-118">b</span></span>|<span data-ttu-id="ac98a-119">Byte</span><span class="sxs-lookup"><span data-stu-id="ac98a-119">Byte</span></span>|<span data-ttu-id="ac98a-120">Blauwert</span><span class="sxs-lookup"><span data-stu-id="ac98a-120">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac98a-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ac98a-121">Relationships</span></span>
<span data-ttu-id="ac98a-122">Keine</span><span class="sxs-lookup"><span data-stu-id="ac98a-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac98a-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ac98a-123">JSON Representation</span></span>
<span data-ttu-id="ac98a-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ac98a-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rgbColor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rgbColor",
  "r": 1024,
  "g": 1024,
  "b": 1024
}
```




