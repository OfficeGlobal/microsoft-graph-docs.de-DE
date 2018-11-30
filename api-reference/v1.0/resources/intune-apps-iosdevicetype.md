---
title: iosDeviceType-Ressourcentyp
description: Enthält die Eigenschaften der möglichen iOS-Gerätetypen, auf denen die mobile App ausgeführt werden kann.
ms.openlocfilehash: b14abbb6713daf9fad7b0d2fd6f7865d251b6147
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018021"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="a0f51-103">iosDeviceType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a0f51-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="a0f51-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a0f51-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0f51-105">Enthält die Eigenschaften der möglichen iOS-Gerätetypen, auf denen die mobile App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="a0f51-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="a0f51-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a0f51-106">Properties</span></span>
|<span data-ttu-id="a0f51-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a0f51-107">Property</span></span>|<span data-ttu-id="a0f51-108">Typ</span><span class="sxs-lookup"><span data-stu-id="a0f51-108">Type</span></span>|<span data-ttu-id="a0f51-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a0f51-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0f51-110">iPad</span><span class="sxs-lookup"><span data-stu-id="a0f51-110">iPad</span></span>|<span data-ttu-id="a0f51-111">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a0f51-111">Boolean</span></span>|<span data-ttu-id="a0f51-112">Gibt an, ob die App auf iPads ausgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="a0f51-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="a0f51-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="a0f51-113">iPhoneAndIPod</span></span>|<span data-ttu-id="a0f51-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a0f51-114">Boolean</span></span>|<span data-ttu-id="a0f51-115">Gibt an, ob die App auf iPhones und iPads ausgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="a0f51-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0f51-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a0f51-116">Relationships</span></span>
<span data-ttu-id="a0f51-117">Keine</span><span class="sxs-lookup"><span data-stu-id="a0f51-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a0f51-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a0f51-118">JSON Representation</span></span>
<span data-ttu-id="a0f51-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a0f51-119">Here is a JSON representation of the resource.</span></span>
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



