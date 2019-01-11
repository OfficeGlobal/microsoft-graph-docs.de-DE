---
title: iosDeviceType-Ressourcentyp
description: Enthält die Eigenschaften der möglichen iOS-Gerätetypen, auf denen die mobile App ausgeführt werden kann.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ffa46d1e8fb693822051250fb4a722815b1dcb73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866780"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="73ecb-103">iosDeviceType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="73ecb-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="73ecb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="73ecb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73ecb-105">Enthält die Eigenschaften der möglichen iOS-Gerätetypen, auf denen die mobile App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="73ecb-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="73ecb-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="73ecb-106">Properties</span></span>
|<span data-ttu-id="73ecb-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="73ecb-107">Property</span></span>|<span data-ttu-id="73ecb-108">Typ</span><span class="sxs-lookup"><span data-stu-id="73ecb-108">Type</span></span>|<span data-ttu-id="73ecb-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73ecb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73ecb-110">iPad</span><span class="sxs-lookup"><span data-stu-id="73ecb-110">iPad</span></span>|<span data-ttu-id="73ecb-111">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="73ecb-111">Boolean</span></span>|<span data-ttu-id="73ecb-112">Gibt an, ob die App auf iPads ausgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="73ecb-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="73ecb-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="73ecb-113">iPhoneAndIPod</span></span>|<span data-ttu-id="73ecb-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="73ecb-114">Boolean</span></span>|<span data-ttu-id="73ecb-115">Gibt an, ob die App auf iPhones und iPads ausgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="73ecb-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73ecb-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="73ecb-116">Relationships</span></span>
<span data-ttu-id="73ecb-117">Keine</span><span class="sxs-lookup"><span data-stu-id="73ecb-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="73ecb-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="73ecb-118">JSON Representation</span></span>
<span data-ttu-id="73ecb-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="73ecb-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceType",
  "iPad": true,
  "iPhoneAndIPod": true
}
```



