---
title: Ressourcentyp mobileAppSupportedDeviceType
description: Eigenschaften des Geräts
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c01691b3f6fcb2ed5838c1c9103c99ad6fbe792f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399752"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="e45d9-103">Ressourcentyp mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="e45d9-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="e45d9-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e45d9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e45d9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e45d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e45d9-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e45d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e45d9-107">Eigenschaften des Geräts</span><span class="sxs-lookup"><span data-stu-id="e45d9-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="e45d9-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e45d9-108">Properties</span></span>
|<span data-ttu-id="e45d9-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e45d9-109">Property</span></span>|<span data-ttu-id="e45d9-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e45d9-110">Type</span></span>|<span data-ttu-id="e45d9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e45d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e45d9-112">type</span><span class="sxs-lookup"><span data-stu-id="e45d9-112">type</span></span>|[<span data-ttu-id="e45d9-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="e45d9-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="e45d9-114">Gerätetyp.</span><span class="sxs-lookup"><span data-stu-id="e45d9-114">Device type.</span></span> <span data-ttu-id="e45d9-115">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="e45d9-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="e45d9-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="e45d9-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="e45d9-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e45d9-117">String</span></span>|<span data-ttu-id="e45d9-118">Minimale Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="e45d9-118">Minimum OS version</span></span>|
|<span data-ttu-id="e45d9-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="e45d9-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="e45d9-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e45d9-120">String</span></span>|<span data-ttu-id="e45d9-121">Maximale Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="e45d9-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="e45d9-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e45d9-122">Relationships</span></span>
<span data-ttu-id="e45d9-123">Keine</span><span class="sxs-lookup"><span data-stu-id="e45d9-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e45d9-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e45d9-124">JSON Representation</span></span>
<span data-ttu-id="e45d9-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e45d9-125">Here is a JSON representation of the resource.</span></span>
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




