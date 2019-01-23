---
title: Ressourcentyp operatingSystemVersionRange
description: Betriebssystem Versionsbereich.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aaac008b013a8bf2cfd1a88d1fab06a523abb949
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398527"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="33833-103">Ressourcentyp operatingSystemVersionRange</span><span class="sxs-lookup"><span data-stu-id="33833-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="33833-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="33833-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="33833-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33833-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33833-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="33833-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33833-107">Betriebssystem Versionsbereich.</span><span class="sxs-lookup"><span data-stu-id="33833-107">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="33833-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="33833-108">Properties</span></span>
|<span data-ttu-id="33833-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="33833-109">Property</span></span>|<span data-ttu-id="33833-110">Typ</span><span class="sxs-lookup"><span data-stu-id="33833-110">Type</span></span>|<span data-ttu-id="33833-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33833-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33833-112">description</span><span class="sxs-lookup"><span data-stu-id="33833-112">description</span></span>|<span data-ttu-id="33833-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33833-113">String</span></span>|<span data-ttu-id="33833-114">Die Beschreibung dieses Bereichs (z. B. gültig 1702 Builds)</span><span class="sxs-lookup"><span data-stu-id="33833-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="33833-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="33833-115">lowestVersion</span></span>|<span data-ttu-id="33833-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33833-116">String</span></span>|<span data-ttu-id="33833-117">Die niedrigste inklusive Version, die dieser Bereich enthält.</span><span class="sxs-lookup"><span data-stu-id="33833-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="33833-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="33833-118">highestVersion</span></span>|<span data-ttu-id="33833-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33833-119">String</span></span>|<span data-ttu-id="33833-120">Die höchste inklusive Version, die dieser Bereich enthält.</span><span class="sxs-lookup"><span data-stu-id="33833-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33833-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="33833-121">Relationships</span></span>
<span data-ttu-id="33833-122">Keine</span><span class="sxs-lookup"><span data-stu-id="33833-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="33833-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="33833-123">JSON Representation</span></span>
<span data-ttu-id="33833-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="33833-124">Here is a JSON representation of the resource.</span></span>
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




