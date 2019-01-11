---
title: Ressourcentyp numberRange
description: Nummern Definition.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5b428320fd66263149b6d443a15c6a0e1eee744a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845703"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="ccfbd-103">Ressourcentyp numberRange</span><span class="sxs-lookup"><span data-stu-id="ccfbd-103">numberRange resource type</span></span>

> <span data-ttu-id="ccfbd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ccfbd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ccfbd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ccfbd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ccfbd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ccfbd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ccfbd-107">Nummern Definition.</span><span class="sxs-lookup"><span data-stu-id="ccfbd-107">Number Range definition.</span></span>
## <a name="properties"></a><span data-ttu-id="ccfbd-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ccfbd-108">Properties</span></span>
|<span data-ttu-id="ccfbd-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ccfbd-109">Property</span></span>|<span data-ttu-id="ccfbd-110">Typ</span><span class="sxs-lookup"><span data-stu-id="ccfbd-110">Type</span></span>|<span data-ttu-id="ccfbd-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ccfbd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccfbd-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="ccfbd-112">lowerNumber</span></span>|<span data-ttu-id="ccfbd-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ccfbd-113">Int32</span></span>|<span data-ttu-id="ccfbd-114">Niedrigere Zahl.</span><span class="sxs-lookup"><span data-stu-id="ccfbd-114">Lower number.</span></span>|
|<span data-ttu-id="ccfbd-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="ccfbd-115">upperNumber</span></span>|<span data-ttu-id="ccfbd-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ccfbd-116">Int32</span></span>|<span data-ttu-id="ccfbd-117">Obergrenze.</span><span class="sxs-lookup"><span data-stu-id="ccfbd-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccfbd-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ccfbd-118">Relationships</span></span>
<span data-ttu-id="ccfbd-119">Keine</span><span class="sxs-lookup"><span data-stu-id="ccfbd-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ccfbd-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ccfbd-120">JSON Representation</span></span>
<span data-ttu-id="ccfbd-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ccfbd-121">Here is a JSON representation of the resource.</span></span>
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





