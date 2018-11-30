---
title: Ressourcentyp numberRange
description: Nummern Definition.
ms.openlocfilehash: ef4b24e3034414221365d81c40b453e7ca66a94b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058480"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="a017b-103">Ressourcentyp numberRange</span><span class="sxs-lookup"><span data-stu-id="a017b-103">numberRange resource type</span></span>

> <span data-ttu-id="a017b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a017b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a017b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a017b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a017b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a017b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a017b-107">Nummern Definition.</span><span class="sxs-lookup"><span data-stu-id="a017b-107">Number Range definition.</span></span>
## <a name="properties"></a><span data-ttu-id="a017b-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a017b-108">Properties</span></span>
|<span data-ttu-id="a017b-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a017b-109">Property</span></span>|<span data-ttu-id="a017b-110">Typ</span><span class="sxs-lookup"><span data-stu-id="a017b-110">Type</span></span>|<span data-ttu-id="a017b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a017b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a017b-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="a017b-112">lowerNumber</span></span>|<span data-ttu-id="a017b-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a017b-113">Int32</span></span>|<span data-ttu-id="a017b-114">Niedrigere Zahl.</span><span class="sxs-lookup"><span data-stu-id="a017b-114">Lower number.</span></span>|
|<span data-ttu-id="a017b-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="a017b-115">upperNumber</span></span>|<span data-ttu-id="a017b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a017b-116">Int32</span></span>|<span data-ttu-id="a017b-117">Obergrenze.</span><span class="sxs-lookup"><span data-stu-id="a017b-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a017b-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a017b-118">Relationships</span></span>
<span data-ttu-id="a017b-119">Keine</span><span class="sxs-lookup"><span data-stu-id="a017b-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a017b-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a017b-120">JSON Representation</span></span>
<span data-ttu-id="a017b-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a017b-121">Here is a JSON representation of the resource.</span></span>
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





