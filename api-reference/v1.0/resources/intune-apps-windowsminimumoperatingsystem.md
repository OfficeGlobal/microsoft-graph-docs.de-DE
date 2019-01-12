---
title: windowsMinimumOperatingSystem-Ressourcentyp
description: Das mindestens für eine mobile Windows-App erforderliche Betriebssystem.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 521b82448d58a831f88bdf9d548612aee86bcba6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972950"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="71d10-103">windowsMinimumOperatingSystem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="71d10-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="71d10-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="71d10-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71d10-105">Das mindestens für eine mobile Windows-App erforderliche Betriebssystem.</span><span class="sxs-lookup"><span data-stu-id="71d10-105">The minimum operating system required for a Windows mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="71d10-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="71d10-106">Properties</span></span>
|<span data-ttu-id="71d10-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71d10-107">Property</span></span>|<span data-ttu-id="71d10-108">Typ</span><span class="sxs-lookup"><span data-stu-id="71d10-108">Type</span></span>|<span data-ttu-id="71d10-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71d10-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71d10-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="71d10-110">v8_0</span></span>|<span data-ttu-id="71d10-111">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="71d10-111">Boolean</span></span>|<span data-ttu-id="71d10-112">Windows-Version 8.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="71d10-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="71d10-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="71d10-113">v8_1</span></span>|<span data-ttu-id="71d10-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="71d10-114">Boolean</span></span>|<span data-ttu-id="71d10-115">Windows-Version 8.1 oder höher</span><span class="sxs-lookup"><span data-stu-id="71d10-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="71d10-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="71d10-116">v10_0</span></span>|<span data-ttu-id="71d10-117">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="71d10-117">Boolean</span></span>|<span data-ttu-id="71d10-118">Windows-Version 10.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="71d10-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71d10-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="71d10-119">Relationships</span></span>
<span data-ttu-id="71d10-120">Keine</span><span class="sxs-lookup"><span data-stu-id="71d10-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="71d10-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="71d10-121">JSON Representation</span></span>
<span data-ttu-id="71d10-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="71d10-122">Here is a JSON representation of the resource.</span></span>
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



