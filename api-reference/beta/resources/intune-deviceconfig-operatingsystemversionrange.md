---
title: Ressourcentyp operatingSystemVersionRange
description: Betriebssystem Versionsbereich.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c0b81482ad4b48ad5fe59b1ec0109fcd3bf03f83
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918546"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="e2e33-103">Ressourcentyp operatingSystemVersionRange</span><span class="sxs-lookup"><span data-stu-id="e2e33-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="e2e33-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e2e33-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2e33-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e2e33-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2e33-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e2e33-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2e33-107">Betriebssystem Versionsbereich.</span><span class="sxs-lookup"><span data-stu-id="e2e33-107">Operating System version range.</span></span>
## <a name="properties"></a><span data-ttu-id="e2e33-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e2e33-108">Properties</span></span>
|<span data-ttu-id="e2e33-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e2e33-109">Property</span></span>|<span data-ttu-id="e2e33-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e2e33-110">Type</span></span>|<span data-ttu-id="e2e33-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2e33-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2e33-112">description</span><span class="sxs-lookup"><span data-stu-id="e2e33-112">description</span></span>|<span data-ttu-id="e2e33-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2e33-113">String</span></span>|<span data-ttu-id="e2e33-114">Die Beschreibung dieses Bereichs (z. B. gültig 1702 Builds)</span><span class="sxs-lookup"><span data-stu-id="e2e33-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="e2e33-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="e2e33-115">lowestVersion</span></span>|<span data-ttu-id="e2e33-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2e33-116">String</span></span>|<span data-ttu-id="e2e33-117">Die niedrigste inklusive Version, die dieser Bereich enthält.</span><span class="sxs-lookup"><span data-stu-id="e2e33-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="e2e33-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="e2e33-118">highestVersion</span></span>|<span data-ttu-id="e2e33-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2e33-119">String</span></span>|<span data-ttu-id="e2e33-120">Die höchste inklusive Version, die dieser Bereich enthält.</span><span class="sxs-lookup"><span data-stu-id="e2e33-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2e33-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e2e33-121">Relationships</span></span>
<span data-ttu-id="e2e33-122">Keine</span><span class="sxs-lookup"><span data-stu-id="e2e33-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e2e33-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e2e33-123">JSON Representation</span></span>
<span data-ttu-id="e2e33-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e2e33-124">Here is a JSON representation of the resource.</span></span>
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





