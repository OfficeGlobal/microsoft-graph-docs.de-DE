---
title: rgbColor-Ressourcentyp
description: Farbe in RGB
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fd734d2cb7c1c03cfdab62b8a8f1acd9acac6814
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846725"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="3c2b4-103">rgbColor-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3c2b4-103">rgbColor resource type</span></span>

> <span data-ttu-id="3c2b4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3c2b4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c2b4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c2b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c2b4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3c2b4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c2b4-107">Farbe in RGB</span><span class="sxs-lookup"><span data-stu-id="3c2b4-107">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="3c2b4-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3c2b4-108">Properties</span></span>
|<span data-ttu-id="3c2b4-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3c2b4-109">Property</span></span>|<span data-ttu-id="3c2b4-110">Typ</span><span class="sxs-lookup"><span data-stu-id="3c2b4-110">Type</span></span>|<span data-ttu-id="3c2b4-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c2b4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c2b4-112">r</span><span class="sxs-lookup"><span data-stu-id="3c2b4-112">r</span></span>|<span data-ttu-id="3c2b4-113">Byte</span><span class="sxs-lookup"><span data-stu-id="3c2b4-113">Byte</span></span>|<span data-ttu-id="3c2b4-114">Rotwert</span><span class="sxs-lookup"><span data-stu-id="3c2b4-114">Red value</span></span>|
|<span data-ttu-id="3c2b4-115">g</span><span class="sxs-lookup"><span data-stu-id="3c2b4-115">g</span></span>|<span data-ttu-id="3c2b4-116">Byte</span><span class="sxs-lookup"><span data-stu-id="3c2b4-116">Byte</span></span>|<span data-ttu-id="3c2b4-117">Grünwert</span><span class="sxs-lookup"><span data-stu-id="3c2b4-117">Green value</span></span>|
|<span data-ttu-id="3c2b4-118">b</span><span class="sxs-lookup"><span data-stu-id="3c2b4-118">b</span></span>|<span data-ttu-id="3c2b4-119">Byte</span><span class="sxs-lookup"><span data-stu-id="3c2b4-119">Byte</span></span>|<span data-ttu-id="3c2b4-120">Blauwert</span><span class="sxs-lookup"><span data-stu-id="3c2b4-120">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c2b4-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3c2b4-121">Relationships</span></span>
<span data-ttu-id="3c2b4-122">Keine</span><span class="sxs-lookup"><span data-stu-id="3c2b4-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3c2b4-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3c2b4-123">JSON Representation</span></span>
<span data-ttu-id="3c2b4-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3c2b4-124">Here is a JSON representation of the resource.</span></span>
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





