---
title: Ressourcentyp operatingSystemVersionRange
description: Betriebssystem Versionsbereich.
author: tfitzmac
ms.openlocfilehash: b853e71b2d8f66d24122afb51cea97fc6a8f8d7e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331164"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="693cd-103">Ressourcentyp operatingSystemVersionRange</span><span class="sxs-lookup"><span data-stu-id="693cd-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="693cd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="693cd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="693cd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="693cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="693cd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="693cd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="693cd-107">Betriebssystem Versionsbereich.</span><span class="sxs-lookup"><span data-stu-id="693cd-107">Operating System version range.</span></span>
## <a name="properties"></a><span data-ttu-id="693cd-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="693cd-108">Properties</span></span>
|<span data-ttu-id="693cd-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="693cd-109">Property</span></span>|<span data-ttu-id="693cd-110">Typ</span><span class="sxs-lookup"><span data-stu-id="693cd-110">Type</span></span>|<span data-ttu-id="693cd-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="693cd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="693cd-112">description</span><span class="sxs-lookup"><span data-stu-id="693cd-112">description</span></span>|<span data-ttu-id="693cd-113">String</span><span class="sxs-lookup"><span data-stu-id="693cd-113">String</span></span>|<span data-ttu-id="693cd-114">Die Beschreibung dieses Bereichs (z. B. gültig 1702 Builds)</span><span class="sxs-lookup"><span data-stu-id="693cd-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="693cd-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="693cd-115">lowestVersion</span></span>|<span data-ttu-id="693cd-116">String</span><span class="sxs-lookup"><span data-stu-id="693cd-116">String</span></span>|<span data-ttu-id="693cd-117">Die niedrigste inklusive Version, die dieser Bereich enthält.</span><span class="sxs-lookup"><span data-stu-id="693cd-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="693cd-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="693cd-118">highestVersion</span></span>|<span data-ttu-id="693cd-119">String</span><span class="sxs-lookup"><span data-stu-id="693cd-119">String</span></span>|<span data-ttu-id="693cd-120">Die höchste inklusive Version, die dieser Bereich enthält.</span><span class="sxs-lookup"><span data-stu-id="693cd-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="693cd-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="693cd-121">Relationships</span></span>
<span data-ttu-id="693cd-122">Keine</span><span class="sxs-lookup"><span data-stu-id="693cd-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="693cd-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="693cd-123">JSON Representation</span></span>
<span data-ttu-id="693cd-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="693cd-124">Here is a JSON representation of the resource.</span></span>
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





