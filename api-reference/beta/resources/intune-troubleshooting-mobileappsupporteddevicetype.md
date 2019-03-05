---
title: mobileAppSupportedDeviceType-Ressourcentyp
description: Geräteeigenschaften
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76b3ca431bc68f93144a33dd8c5e8e5f036764a0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140579"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="c7b26-103">mobileAppSupportedDeviceType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c7b26-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="c7b26-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c7b26-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7b26-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c7b26-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7b26-106">Geräteeigenschaften</span><span class="sxs-lookup"><span data-stu-id="c7b26-106">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="c7b26-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c7b26-107">Properties</span></span>
|<span data-ttu-id="c7b26-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c7b26-108">Property</span></span>|<span data-ttu-id="c7b26-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c7b26-109">Type</span></span>|<span data-ttu-id="c7b26-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7b26-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7b26-111">type</span><span class="sxs-lookup"><span data-stu-id="c7b26-111">type</span></span>|[<span data-ttu-id="c7b26-112">deviceType</span><span class="sxs-lookup"><span data-stu-id="c7b26-112">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="c7b26-113">Gerätetyp.</span><span class="sxs-lookup"><span data-stu-id="c7b26-113">Device type.</span></span> <span data-ttu-id="c7b26-114">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6` `nokia` `windowsPhone` `mac` `winCE` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM`,,,,,,,, `holoLens`,, `androidEnterprise` ,,,,,, `surfaceHub` `androidForWork` `winEmbedded` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c7b26-114">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="c7b26-115">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="c7b26-115">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="c7b26-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c7b26-116">String</span></span>|<span data-ttu-id="c7b26-117">Minimale Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="c7b26-117">Minimum OS version</span></span>|
|<span data-ttu-id="c7b26-118">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="c7b26-118">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="c7b26-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c7b26-119">String</span></span>|<span data-ttu-id="c7b26-120">Maximale Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="c7b26-120">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7b26-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c7b26-121">Relationships</span></span>
<span data-ttu-id="c7b26-122">Keine</span><span class="sxs-lookup"><span data-stu-id="c7b26-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7b26-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c7b26-123">JSON Representation</span></span>
<span data-ttu-id="c7b26-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c7b26-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppSupportedDeviceType",
  "type": "String",
  "minimumOperatingSystemVersion": "String",
  "maximumOperatingSystemVersion": "String"
}
```




