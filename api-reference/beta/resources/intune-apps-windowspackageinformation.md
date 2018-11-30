---
title: Ressourcentyp windowsPackageInformation
description: Enthält Eigenschaften für die Paketinformationen für einen Windows-Geschäfts-app.
ms.openlocfilehash: a7676320d5aa2eeab1140e6cc631c4061d2c5d14
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062556"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="49811-103">Ressourcentyp windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="49811-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="49811-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="49811-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49811-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="49811-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49811-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="49811-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49811-107">Enthält Eigenschaften für die Paketinformationen für einen Windows-Geschäfts-app.</span><span class="sxs-lookup"><span data-stu-id="49811-107">Contains properties for the package information for a Windows line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="49811-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="49811-108">Properties</span></span>
|<span data-ttu-id="49811-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="49811-109">Property</span></span>|<span data-ttu-id="49811-110">Typ</span><span class="sxs-lookup"><span data-stu-id="49811-110">Type</span></span>|<span data-ttu-id="49811-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49811-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49811-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="49811-112">applicableArchitecture</span></span>|[<span data-ttu-id="49811-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="49811-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="49811-114">Die Windows-Architektur für die diese app ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="49811-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="49811-115">Mögliche Werte sind: `none`, `x86`, `x64`, `arm` und `neutral`.</span><span class="sxs-lookup"><span data-stu-id="49811-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="49811-116">displayName</span><span class="sxs-lookup"><span data-stu-id="49811-116">displayName</span></span>|<span data-ttu-id="49811-117">String</span><span class="sxs-lookup"><span data-stu-id="49811-117">String</span></span>|<span data-ttu-id="49811-118">Der Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="49811-118">The Display Name.</span></span>|
|<span data-ttu-id="49811-119">identityName</span><span class="sxs-lookup"><span data-stu-id="49811-119">identityName</span></span>|<span data-ttu-id="49811-120">String</span><span class="sxs-lookup"><span data-stu-id="49811-120">String</span></span>|<span data-ttu-id="49811-121">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="49811-121">The Identity Name.</span></span>|
|<span data-ttu-id="49811-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="49811-122">identityPublisher</span></span>|<span data-ttu-id="49811-123">String</span><span class="sxs-lookup"><span data-stu-id="49811-123">String</span></span>|<span data-ttu-id="49811-124">Der Identity-Herausgeber.</span><span class="sxs-lookup"><span data-stu-id="49811-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="49811-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="49811-125">identityResourceIdentifier</span></span>|<span data-ttu-id="49811-126">String</span><span class="sxs-lookup"><span data-stu-id="49811-126">String</span></span>|<span data-ttu-id="49811-127">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="49811-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="49811-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="49811-128">identityVersion</span></span>|<span data-ttu-id="49811-129">String</span><span class="sxs-lookup"><span data-stu-id="49811-129">String</span></span>|<span data-ttu-id="49811-130">Die Identität-Version.</span><span class="sxs-lookup"><span data-stu-id="49811-130">The Identity Version.</span></span>|
|<span data-ttu-id="49811-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="49811-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="49811-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="49811-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="49811-133">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="49811-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49811-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="49811-134">Relationships</span></span>
<span data-ttu-id="49811-135">Keine</span><span class="sxs-lookup"><span data-stu-id="49811-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="49811-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="49811-136">JSON Representation</span></span>
<span data-ttu-id="49811-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="49811-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsPackageInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPackageInformation",
  "applicableArchitecture": "String",
  "displayName": "String",
  "identityName": "String",
  "identityPublisher": "String",
  "identityResourceIdentifier": "String",
  "identityVersion": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  }
}
```





