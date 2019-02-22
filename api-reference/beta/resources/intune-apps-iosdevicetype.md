---
title: iosDeviceType-Ressourcentyp
description: Enthält die Eigenschaften der möglichen iOS-Gerätetypen, auf denen die mobile App ausgeführt werden kann.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 72cb6cc19b36c345e66230c7ac1d907c599dcce4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161362"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="64c3e-103">iosDeviceType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="64c3e-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="64c3e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="64c3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64c3e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="64c3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64c3e-106">Enthält die Eigenschaften der möglichen iOS-Gerätetypen, auf denen die mobile App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="64c3e-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="64c3e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="64c3e-107">Properties</span></span>
|<span data-ttu-id="64c3e-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="64c3e-108">Property</span></span>|<span data-ttu-id="64c3e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="64c3e-109">Type</span></span>|<span data-ttu-id="64c3e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64c3e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64c3e-111">iPad</span><span class="sxs-lookup"><span data-stu-id="64c3e-111">iPad</span></span>|<span data-ttu-id="64c3e-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="64c3e-112">Boolean</span></span>|<span data-ttu-id="64c3e-113">Gibt an, ob die App auf iPads ausgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="64c3e-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="64c3e-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="64c3e-114">iPhoneAndIPod</span></span>|<span data-ttu-id="64c3e-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="64c3e-115">Boolean</span></span>|<span data-ttu-id="64c3e-116">Gibt an, ob die App auf iPhones und iPads ausgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="64c3e-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64c3e-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="64c3e-117">Relationships</span></span>
<span data-ttu-id="64c3e-118">Keine</span><span class="sxs-lookup"><span data-stu-id="64c3e-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64c3e-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="64c3e-119">JSON Representation</span></span>
<span data-ttu-id="64c3e-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="64c3e-120">Here is a JSON representation of the resource.</span></span>
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




