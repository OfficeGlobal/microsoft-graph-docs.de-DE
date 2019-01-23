---
title: iosDeviceType-Ressourcentyp
description: Enthält die Eigenschaften der möglichen iOS-Gerätetypen, auf denen die mobile App ausgeführt werden kann.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b68c7ce163dbf0f9232bf53d919ae84c7906c997
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395384"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="948fc-103">iosDeviceType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="948fc-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="948fc-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="948fc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="948fc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="948fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="948fc-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="948fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="948fc-107">Enthält die Eigenschaften der möglichen iOS-Gerätetypen, auf denen die mobile App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="948fc-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="948fc-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="948fc-108">Properties</span></span>
|<span data-ttu-id="948fc-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="948fc-109">Property</span></span>|<span data-ttu-id="948fc-110">Typ</span><span class="sxs-lookup"><span data-stu-id="948fc-110">Type</span></span>|<span data-ttu-id="948fc-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="948fc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="948fc-112">iPad</span><span class="sxs-lookup"><span data-stu-id="948fc-112">iPad</span></span>|<span data-ttu-id="948fc-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="948fc-113">Boolean</span></span>|<span data-ttu-id="948fc-114">Gibt an, ob die App auf iPads ausgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="948fc-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="948fc-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="948fc-115">iPhoneAndIPod</span></span>|<span data-ttu-id="948fc-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="948fc-116">Boolean</span></span>|<span data-ttu-id="948fc-117">Gibt an, ob die App auf iPhones und iPads ausgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="948fc-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="948fc-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="948fc-118">Relationships</span></span>
<span data-ttu-id="948fc-119">Keine</span><span class="sxs-lookup"><span data-stu-id="948fc-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="948fc-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="948fc-120">JSON Representation</span></span>
<span data-ttu-id="948fc-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="948fc-121">Here is a JSON representation of the resource.</span></span>
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




