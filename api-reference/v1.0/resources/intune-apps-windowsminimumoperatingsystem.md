---
title: windowsMinimumOperatingSystem-Ressourcentyp
description: Das mindestens für eine mobile Windows-App erforderliche Betriebssystem.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f337a61f3a0cfd52e042e65bb3d8de57dcf9f283
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254464"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="dddb6-103">windowsMinimumOperatingSystem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dddb6-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="dddb6-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="dddb6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dddb6-105">Das mindestens für eine mobile Windows-App erforderliche Betriebssystem.</span><span class="sxs-lookup"><span data-stu-id="dddb6-105">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="dddb6-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dddb6-106">Properties</span></span>
|<span data-ttu-id="dddb6-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dddb6-107">Property</span></span>|<span data-ttu-id="dddb6-108">Typ</span><span class="sxs-lookup"><span data-stu-id="dddb6-108">Type</span></span>|<span data-ttu-id="dddb6-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dddb6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dddb6-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="dddb6-110">v8_0</span></span>|<span data-ttu-id="dddb6-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="dddb6-111">Boolean</span></span>|<span data-ttu-id="dddb6-112">Windows-Version 8.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="dddb6-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="dddb6-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="dddb6-113">v8_1</span></span>|<span data-ttu-id="dddb6-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="dddb6-114">Boolean</span></span>|<span data-ttu-id="dddb6-115">Windows-Version 8.1 oder höher</span><span class="sxs-lookup"><span data-stu-id="dddb6-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="dddb6-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="dddb6-116">v10_0</span></span>|<span data-ttu-id="dddb6-117">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dddb6-117">Boolean</span></span>|<span data-ttu-id="dddb6-118">Windows-Version 10.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="dddb6-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dddb6-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="dddb6-119">Relationships</span></span>
<span data-ttu-id="dddb6-120">Keine</span><span class="sxs-lookup"><span data-stu-id="dddb6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dddb6-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dddb6-121">JSON Representation</span></span>
<span data-ttu-id="dddb6-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dddb6-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true
}
```



