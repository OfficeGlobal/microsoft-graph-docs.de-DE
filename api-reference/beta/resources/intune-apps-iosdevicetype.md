---
title: iosDeviceType-Ressourcentyp
description: Enthält die Eigenschaften der möglichen iOS-Gerätetypen, auf denen die mobile App ausgeführt werden kann.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2fe1f686052468bbab5d7115541a631b77073d6e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977164"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="954e8-103">iosDeviceType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="954e8-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="954e8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="954e8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="954e8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="954e8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="954e8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="954e8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="954e8-107">Enthält die Eigenschaften der möglichen iOS-Gerätetypen, auf denen die mobile App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="954e8-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="954e8-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="954e8-108">Properties</span></span>
|<span data-ttu-id="954e8-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="954e8-109">Property</span></span>|<span data-ttu-id="954e8-110">Typ</span><span class="sxs-lookup"><span data-stu-id="954e8-110">Type</span></span>|<span data-ttu-id="954e8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="954e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="954e8-112">iPad</span><span class="sxs-lookup"><span data-stu-id="954e8-112">iPad</span></span>|<span data-ttu-id="954e8-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="954e8-113">Boolean</span></span>|<span data-ttu-id="954e8-114">Gibt an, ob die App auf iPads ausgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="954e8-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="954e8-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="954e8-115">iPhoneAndIPod</span></span>|<span data-ttu-id="954e8-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="954e8-116">Boolean</span></span>|<span data-ttu-id="954e8-117">Gibt an, ob die App auf iPhones und iPads ausgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="954e8-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="954e8-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="954e8-118">Relationships</span></span>
<span data-ttu-id="954e8-119">Keine</span><span class="sxs-lookup"><span data-stu-id="954e8-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="954e8-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="954e8-120">JSON Representation</span></span>
<span data-ttu-id="954e8-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="954e8-121">Here is a JSON representation of the resource.</span></span>
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





