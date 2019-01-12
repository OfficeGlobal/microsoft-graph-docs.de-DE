---
title: Ressourcentyp numberRange
description: Nummern Definition.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9dc10caaa125144944cf3e6c52c65e58f9d57975
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977408"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="b396d-103">Ressourcentyp numberRange</span><span class="sxs-lookup"><span data-stu-id="b396d-103">numberRange resource type</span></span>

> <span data-ttu-id="b396d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b396d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b396d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b396d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b396d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b396d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b396d-107">Nummern Definition.</span><span class="sxs-lookup"><span data-stu-id="b396d-107">Number Range definition.</span></span>
## <a name="properties"></a><span data-ttu-id="b396d-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b396d-108">Properties</span></span>
|<span data-ttu-id="b396d-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b396d-109">Property</span></span>|<span data-ttu-id="b396d-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b396d-110">Type</span></span>|<span data-ttu-id="b396d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b396d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b396d-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="b396d-112">lowerNumber</span></span>|<span data-ttu-id="b396d-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b396d-113">Int32</span></span>|<span data-ttu-id="b396d-114">Niedrigere Zahl.</span><span class="sxs-lookup"><span data-stu-id="b396d-114">Lower number.</span></span>|
|<span data-ttu-id="b396d-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="b396d-115">upperNumber</span></span>|<span data-ttu-id="b396d-116">Int32</span><span class="sxs-lookup"><span data-stu-id="b396d-116">Int32</span></span>|<span data-ttu-id="b396d-117">Obergrenze.</span><span class="sxs-lookup"><span data-stu-id="b396d-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b396d-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b396d-118">Relationships</span></span>
<span data-ttu-id="b396d-119">Keine</span><span class="sxs-lookup"><span data-stu-id="b396d-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b396d-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b396d-120">JSON Representation</span></span>
<span data-ttu-id="b396d-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b396d-121">Here is a JSON representation of the resource.</span></span>
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





