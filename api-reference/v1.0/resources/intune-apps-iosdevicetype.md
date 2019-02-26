---
title: iosDeviceType-Ressourcentyp
description: Enthält die Eigenschaften der möglichen iOS-Gerätetypen, auf denen die mobile App ausgeführt werden kann.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f3bd1d0aff7e09d5828496de348805075d0b330
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259745"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="950ab-103">iosDeviceType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="950ab-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="950ab-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="950ab-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="950ab-105">Enthält die Eigenschaften der möglichen iOS-Gerätetypen, auf denen die mobile App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="950ab-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="950ab-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="950ab-106">Properties</span></span>
|<span data-ttu-id="950ab-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="950ab-107">Property</span></span>|<span data-ttu-id="950ab-108">Typ</span><span class="sxs-lookup"><span data-stu-id="950ab-108">Type</span></span>|<span data-ttu-id="950ab-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="950ab-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="950ab-110">iPad</span><span class="sxs-lookup"><span data-stu-id="950ab-110">iPad</span></span>|<span data-ttu-id="950ab-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="950ab-111">Boolean</span></span>|<span data-ttu-id="950ab-112">Gibt an, ob die App auf iPads ausgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="950ab-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="950ab-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="950ab-113">iPhoneAndIPod</span></span>|<span data-ttu-id="950ab-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="950ab-114">Boolean</span></span>|<span data-ttu-id="950ab-115">Gibt an, ob die App auf iPhones und iPads ausgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="950ab-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="950ab-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="950ab-116">Relationships</span></span>
<span data-ttu-id="950ab-117">Keine</span><span class="sxs-lookup"><span data-stu-id="950ab-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="950ab-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="950ab-118">JSON Representation</span></span>
<span data-ttu-id="950ab-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="950ab-119">Here is a JSON representation of the resource.</span></span>
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



