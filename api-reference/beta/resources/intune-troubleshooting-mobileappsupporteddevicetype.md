---
title: Ressourcentyp mobileAppSupportedDeviceType
description: Eigenschaften des Geräts
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b1b757e9c621f77d1a26251345ee6751eca2ca7c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980223"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="46ccb-103">Ressourcentyp mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="46ccb-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="46ccb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="46ccb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46ccb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="46ccb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46ccb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="46ccb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46ccb-107">Eigenschaften des Geräts</span><span class="sxs-lookup"><span data-stu-id="46ccb-107">Device properties</span></span>
## <a name="properties"></a><span data-ttu-id="46ccb-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="46ccb-108">Properties</span></span>
|<span data-ttu-id="46ccb-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="46ccb-109">Property</span></span>|<span data-ttu-id="46ccb-110">Typ</span><span class="sxs-lookup"><span data-stu-id="46ccb-110">Type</span></span>|<span data-ttu-id="46ccb-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46ccb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46ccb-112">type</span><span class="sxs-lookup"><span data-stu-id="46ccb-112">type</span></span>|[<span data-ttu-id="46ccb-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="46ccb-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="46ccb-114">Gerätetyp.</span><span class="sxs-lookup"><span data-stu-id="46ccb-114">Device type.</span></span> <span data-ttu-id="46ccb-115">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="46ccb-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="46ccb-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="46ccb-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="46ccb-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="46ccb-117">String</span></span>|<span data-ttu-id="46ccb-118">Minimale Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="46ccb-118">Minimum OS version</span></span>|
|<span data-ttu-id="46ccb-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="46ccb-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="46ccb-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="46ccb-120">String</span></span>|<span data-ttu-id="46ccb-121">Maximale Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="46ccb-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="46ccb-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="46ccb-122">Relationships</span></span>
<span data-ttu-id="46ccb-123">Keine</span><span class="sxs-lookup"><span data-stu-id="46ccb-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="46ccb-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="46ccb-124">JSON Representation</span></span>
<span data-ttu-id="46ccb-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="46ccb-125">Here is a JSON representation of the resource.</span></span>
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





