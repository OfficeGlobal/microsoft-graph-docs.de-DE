---
title: Ressourcentyp mobileAppSupportedDeviceType
description: Eigenschaften des Geräts
ms.openlocfilehash: 7bea84a009d8940608c82bbb551c2d3c8be750ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060510"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="6b0d3-103">Ressourcentyp mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="6b0d3-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="6b0d3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6b0d3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b0d3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6b0d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b0d3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6b0d3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b0d3-107">Eigenschaften des Geräts</span><span class="sxs-lookup"><span data-stu-id="6b0d3-107">Device properties</span></span>
## <a name="properties"></a><span data-ttu-id="6b0d3-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6b0d3-108">Properties</span></span>
|<span data-ttu-id="6b0d3-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6b0d3-109">Property</span></span>|<span data-ttu-id="6b0d3-110">Typ</span><span class="sxs-lookup"><span data-stu-id="6b0d3-110">Type</span></span>|<span data-ttu-id="6b0d3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b0d3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b0d3-112">Typ</span><span class="sxs-lookup"><span data-stu-id="6b0d3-112">type</span></span>|[<span data-ttu-id="6b0d3-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="6b0d3-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="6b0d3-114">Gerätetyp.</span><span class="sxs-lookup"><span data-stu-id="6b0d3-114">Device type.</span></span> <span data-ttu-id="6b0d3-115">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="6b0d3-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="6b0d3-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="6b0d3-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="6b0d3-117">String</span><span class="sxs-lookup"><span data-stu-id="6b0d3-117">String</span></span>|<span data-ttu-id="6b0d3-118">Minimale Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="6b0d3-118">Minimum OS version</span></span>|
|<span data-ttu-id="6b0d3-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="6b0d3-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="6b0d3-120">String</span><span class="sxs-lookup"><span data-stu-id="6b0d3-120">String</span></span>|<span data-ttu-id="6b0d3-121">Maximale Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="6b0d3-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b0d3-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6b0d3-122">Relationships</span></span>
<span data-ttu-id="6b0d3-123">Keine</span><span class="sxs-lookup"><span data-stu-id="6b0d3-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6b0d3-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6b0d3-124">JSON Representation</span></span>
<span data-ttu-id="6b0d3-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6b0d3-125">Here is a JSON representation of the resource.</span></span>
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





