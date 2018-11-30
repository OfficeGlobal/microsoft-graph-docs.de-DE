---
title: windowsMinimumOperatingSystem-Ressourcentyp
description: Das mindestens für eine mobile Windows-App erforderliche Betriebssystem.
ms.openlocfilehash: 077ac386c9f40ca4426f98490241015072b487f7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019462"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="5490e-103">windowsMinimumOperatingSystem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5490e-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="5490e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5490e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5490e-105">Das mindestens für eine mobile Windows-App erforderliche Betriebssystem.</span><span class="sxs-lookup"><span data-stu-id="5490e-105">The minimum operating system required for a Windows mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="5490e-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5490e-106">Properties</span></span>
|<span data-ttu-id="5490e-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5490e-107">Property</span></span>|<span data-ttu-id="5490e-108">Typ</span><span class="sxs-lookup"><span data-stu-id="5490e-108">Type</span></span>|<span data-ttu-id="5490e-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5490e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5490e-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="5490e-110">v8_0</span></span>|<span data-ttu-id="5490e-111">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5490e-111">Boolean</span></span>|<span data-ttu-id="5490e-112">Windows-Version 8.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="5490e-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="5490e-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="5490e-113">v8_1</span></span>|<span data-ttu-id="5490e-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5490e-114">Boolean</span></span>|<span data-ttu-id="5490e-115">Windows-Version 8.1 oder höher</span><span class="sxs-lookup"><span data-stu-id="5490e-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="5490e-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="5490e-116">v10_0</span></span>|<span data-ttu-id="5490e-117">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5490e-117">Boolean</span></span>|<span data-ttu-id="5490e-118">Windows-Version 10.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="5490e-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5490e-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5490e-119">Relationships</span></span>
<span data-ttu-id="5490e-120">Keine</span><span class="sxs-lookup"><span data-stu-id="5490e-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5490e-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5490e-121">JSON Representation</span></span>
<span data-ttu-id="5490e-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5490e-122">Here is a JSON representation of the resource.</span></span>
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



