---
title: rgbColor-Ressourcentyp
description: Farbe in RGB
ms.openlocfilehash: 7b5d450c0126e043a78a6c4f9f0e2fe6f06c7c13
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063960"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="05e87-103">rgbColor-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="05e87-103">rgbColor resource type</span></span>

> <span data-ttu-id="05e87-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="05e87-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05e87-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="05e87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05e87-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="05e87-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05e87-107">Farbe in RGB</span><span class="sxs-lookup"><span data-stu-id="05e87-107">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="05e87-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="05e87-108">Properties</span></span>
|<span data-ttu-id="05e87-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="05e87-109">Property</span></span>|<span data-ttu-id="05e87-110">Typ</span><span class="sxs-lookup"><span data-stu-id="05e87-110">Type</span></span>|<span data-ttu-id="05e87-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="05e87-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05e87-112">r</span><span class="sxs-lookup"><span data-stu-id="05e87-112">r</span></span>|<span data-ttu-id="05e87-113">Byte</span><span class="sxs-lookup"><span data-stu-id="05e87-113">Byte</span></span>|<span data-ttu-id="05e87-114">Rotwert</span><span class="sxs-lookup"><span data-stu-id="05e87-114">Red value</span></span>|
|<span data-ttu-id="05e87-115">g</span><span class="sxs-lookup"><span data-stu-id="05e87-115">g</span></span>|<span data-ttu-id="05e87-116">Byte</span><span class="sxs-lookup"><span data-stu-id="05e87-116">Byte</span></span>|<span data-ttu-id="05e87-117">Grünwert</span><span class="sxs-lookup"><span data-stu-id="05e87-117">Green value</span></span>|
|<span data-ttu-id="05e87-118">b</span><span class="sxs-lookup"><span data-stu-id="05e87-118">b</span></span>|<span data-ttu-id="05e87-119">Byte</span><span class="sxs-lookup"><span data-stu-id="05e87-119">Byte</span></span>|<span data-ttu-id="05e87-120">Blauwert</span><span class="sxs-lookup"><span data-stu-id="05e87-120">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="05e87-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="05e87-121">Relationships</span></span>
<span data-ttu-id="05e87-122">Keine</span><span class="sxs-lookup"><span data-stu-id="05e87-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="05e87-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="05e87-123">JSON Representation</span></span>
<span data-ttu-id="05e87-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="05e87-124">Here is a JSON representation of the resource.</span></span>
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





