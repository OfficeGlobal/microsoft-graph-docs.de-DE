---
title: iosDeviceType-Ressourcentyp
description: Enthält die Eigenschaften der möglichen iOS-Gerätetypen, auf denen die mobile App ausgeführt werden kann.
author: tfitzmac
ms.openlocfilehash: 3111bc4b5fc78f6ed60b4a241b48e443923f7159
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313601"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="8fe1b-103">iosDeviceType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8fe1b-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="8fe1b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8fe1b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8fe1b-105">Enthält die Eigenschaften der möglichen iOS-Gerätetypen, auf denen die mobile App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="8fe1b-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="8fe1b-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8fe1b-106">Properties</span></span>
|<span data-ttu-id="8fe1b-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8fe1b-107">Property</span></span>|<span data-ttu-id="8fe1b-108">Typ</span><span class="sxs-lookup"><span data-stu-id="8fe1b-108">Type</span></span>|<span data-ttu-id="8fe1b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8fe1b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fe1b-110">iPad</span><span class="sxs-lookup"><span data-stu-id="8fe1b-110">iPad</span></span>|<span data-ttu-id="8fe1b-111">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8fe1b-111">Boolean</span></span>|<span data-ttu-id="8fe1b-112">Gibt an, ob die App auf iPads ausgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="8fe1b-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="8fe1b-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="8fe1b-113">iPhoneAndIPod</span></span>|<span data-ttu-id="8fe1b-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8fe1b-114">Boolean</span></span>|<span data-ttu-id="8fe1b-115">Gibt an, ob die App auf iPhones und iPads ausgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="8fe1b-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fe1b-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8fe1b-116">Relationships</span></span>
<span data-ttu-id="8fe1b-117">Keine</span><span class="sxs-lookup"><span data-stu-id="8fe1b-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8fe1b-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8fe1b-118">JSON Representation</span></span>
<span data-ttu-id="8fe1b-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8fe1b-119">Here is a JSON representation of the resource.</span></span>
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



