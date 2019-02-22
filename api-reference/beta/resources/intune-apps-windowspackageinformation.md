---
title: Dem windowspackageinformation-Ressourcentyp
description: Enthält Eigenschaften für die Paketinformationen für eine Windows-Branchen-app.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba69fe277809b3ce4d6f81a198fc305204984d73
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166451"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="68c41-103">Dem windowspackageinformation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="68c41-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="68c41-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="68c41-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68c41-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="68c41-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68c41-106">Enthält Eigenschaften für die Paketinformationen für eine Windows-Branchen-app.</span><span class="sxs-lookup"><span data-stu-id="68c41-106">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="68c41-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="68c41-107">Properties</span></span>
|<span data-ttu-id="68c41-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="68c41-108">Property</span></span>|<span data-ttu-id="68c41-109">Typ</span><span class="sxs-lookup"><span data-stu-id="68c41-109">Type</span></span>|<span data-ttu-id="68c41-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68c41-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68c41-111">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="68c41-111">applicableArchitecture</span></span>|[<span data-ttu-id="68c41-112">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="68c41-112">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="68c41-113">Die Windows-Architektur, für die diese APP ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="68c41-113">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="68c41-114">Mögliche Werte sind: `none`, `x86`, `x64`, `arm`, `neutral` und `arm64`.</span><span class="sxs-lookup"><span data-stu-id="68c41-114">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="68c41-115">displayName</span><span class="sxs-lookup"><span data-stu-id="68c41-115">displayName</span></span>|<span data-ttu-id="68c41-116">String</span><span class="sxs-lookup"><span data-stu-id="68c41-116">String</span></span>|<span data-ttu-id="68c41-117">Der Anzeige Name.</span><span class="sxs-lookup"><span data-stu-id="68c41-117">The Display Name.</span></span>|
|<span data-ttu-id="68c41-118">identityName</span><span class="sxs-lookup"><span data-stu-id="68c41-118">identityName</span></span>|<span data-ttu-id="68c41-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="68c41-119">String</span></span>|<span data-ttu-id="68c41-120">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="68c41-120">The Identity Name.</span></span>|
|<span data-ttu-id="68c41-121">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="68c41-121">identityPublisher</span></span>|<span data-ttu-id="68c41-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="68c41-122">String</span></span>|<span data-ttu-id="68c41-123">Der Identitäts Herausgeber.</span><span class="sxs-lookup"><span data-stu-id="68c41-123">The Identity Publisher.</span></span>|
|<span data-ttu-id="68c41-124">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="68c41-124">identityResourceIdentifier</span></span>|<span data-ttu-id="68c41-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="68c41-125">String</span></span>|<span data-ttu-id="68c41-126">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="68c41-126">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="68c41-127">identityVersion</span><span class="sxs-lookup"><span data-stu-id="68c41-127">identityVersion</span></span>|<span data-ttu-id="68c41-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="68c41-128">String</span></span>|<span data-ttu-id="68c41-129">Die Identitäts Version.</span><span class="sxs-lookup"><span data-stu-id="68c41-129">The Identity Version.</span></span>|
|<span data-ttu-id="68c41-130">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="68c41-130">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="68c41-131">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="68c41-131">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="68c41-132">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="68c41-132">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68c41-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="68c41-133">Relationships</span></span>
<span data-ttu-id="68c41-134">Keine</span><span class="sxs-lookup"><span data-stu-id="68c41-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68c41-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="68c41-135">JSON Representation</span></span>
<span data-ttu-id="68c41-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="68c41-136">Here is a JSON representation of the resource.</span></span>
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




