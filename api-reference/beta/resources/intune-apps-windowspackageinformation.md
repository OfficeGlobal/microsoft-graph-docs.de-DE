---
title: Ressourcentyp windowsPackageInformation
description: Enthält Eigenschaften für die Paketinformationen für einen Windows-Geschäfts-app.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0f7f3cd593670e071ae62bdb287bcebeee01d555
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849532"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="9fa59-103">Ressourcentyp windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="9fa59-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="9fa59-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9fa59-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fa59-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9fa59-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9fa59-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9fa59-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9fa59-107">Enthält Eigenschaften für die Paketinformationen für einen Windows-Geschäfts-app.</span><span class="sxs-lookup"><span data-stu-id="9fa59-107">Contains properties for the package information for a Windows line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="9fa59-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9fa59-108">Properties</span></span>
|<span data-ttu-id="9fa59-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9fa59-109">Property</span></span>|<span data-ttu-id="9fa59-110">Typ</span><span class="sxs-lookup"><span data-stu-id="9fa59-110">Type</span></span>|<span data-ttu-id="9fa59-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9fa59-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fa59-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="9fa59-112">applicableArchitecture</span></span>|[<span data-ttu-id="9fa59-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="9fa59-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="9fa59-114">Die Windows-Architektur für die diese app ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="9fa59-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="9fa59-115">Mögliche Werte sind: `none`, `x86`, `x64`, `arm` und `neutral`.</span><span class="sxs-lookup"><span data-stu-id="9fa59-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="9fa59-116">displayName</span><span class="sxs-lookup"><span data-stu-id="9fa59-116">displayName</span></span>|<span data-ttu-id="9fa59-117">String</span><span class="sxs-lookup"><span data-stu-id="9fa59-117">String</span></span>|<span data-ttu-id="9fa59-118">Der Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="9fa59-118">The Display Name.</span></span>|
|<span data-ttu-id="9fa59-119">identityName</span><span class="sxs-lookup"><span data-stu-id="9fa59-119">identityName</span></span>|<span data-ttu-id="9fa59-120">String</span><span class="sxs-lookup"><span data-stu-id="9fa59-120">String</span></span>|<span data-ttu-id="9fa59-121">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="9fa59-121">The Identity Name.</span></span>|
|<span data-ttu-id="9fa59-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="9fa59-122">identityPublisher</span></span>|<span data-ttu-id="9fa59-123">String</span><span class="sxs-lookup"><span data-stu-id="9fa59-123">String</span></span>|<span data-ttu-id="9fa59-124">Der Identity-Herausgeber.</span><span class="sxs-lookup"><span data-stu-id="9fa59-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="9fa59-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="9fa59-125">identityResourceIdentifier</span></span>|<span data-ttu-id="9fa59-126">String</span><span class="sxs-lookup"><span data-stu-id="9fa59-126">String</span></span>|<span data-ttu-id="9fa59-127">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="9fa59-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="9fa59-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="9fa59-128">identityVersion</span></span>|<span data-ttu-id="9fa59-129">String</span><span class="sxs-lookup"><span data-stu-id="9fa59-129">String</span></span>|<span data-ttu-id="9fa59-130">Die Identität-Version.</span><span class="sxs-lookup"><span data-stu-id="9fa59-130">The Identity Version.</span></span>|
|<span data-ttu-id="9fa59-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9fa59-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9fa59-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9fa59-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="9fa59-133">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="9fa59-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fa59-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9fa59-134">Relationships</span></span>
<span data-ttu-id="9fa59-135">Keine</span><span class="sxs-lookup"><span data-stu-id="9fa59-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9fa59-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9fa59-136">JSON Representation</span></span>
<span data-ttu-id="9fa59-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9fa59-137">Here is a JSON representation of the resource.</span></span>
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





