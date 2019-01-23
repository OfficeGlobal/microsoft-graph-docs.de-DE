---
title: Ressourcentyp windowsPackageInformation
description: Enthält Eigenschaften für die Paketinformationen für einen Windows-Geschäfts-app.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 112d84c5bae889e24b889b4598d61a6b3d63db50
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403280"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="78649-103">Ressourcentyp windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="78649-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="78649-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="78649-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="78649-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="78649-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78649-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="78649-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78649-107">Enthält Eigenschaften für die Paketinformationen für einen Windows-Geschäfts-app.</span><span class="sxs-lookup"><span data-stu-id="78649-107">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="78649-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="78649-108">Properties</span></span>
|<span data-ttu-id="78649-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="78649-109">Property</span></span>|<span data-ttu-id="78649-110">Typ</span><span class="sxs-lookup"><span data-stu-id="78649-110">Type</span></span>|<span data-ttu-id="78649-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78649-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78649-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="78649-112">applicableArchitecture</span></span>|[<span data-ttu-id="78649-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="78649-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="78649-114">Die Windows-Architektur für die diese app ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="78649-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="78649-115">Mögliche Werte sind: `none`, `x86`, `x64`, `arm`, `neutral` und `arm64`.</span><span class="sxs-lookup"><span data-stu-id="78649-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="78649-116">displayName</span><span class="sxs-lookup"><span data-stu-id="78649-116">displayName</span></span>|<span data-ttu-id="78649-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="78649-117">String</span></span>|<span data-ttu-id="78649-118">Der Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="78649-118">The Display Name.</span></span>|
|<span data-ttu-id="78649-119">identityName</span><span class="sxs-lookup"><span data-stu-id="78649-119">identityName</span></span>|<span data-ttu-id="78649-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="78649-120">String</span></span>|<span data-ttu-id="78649-121">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="78649-121">The Identity Name.</span></span>|
|<span data-ttu-id="78649-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="78649-122">identityPublisher</span></span>|<span data-ttu-id="78649-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="78649-123">String</span></span>|<span data-ttu-id="78649-124">Der Identity-Herausgeber.</span><span class="sxs-lookup"><span data-stu-id="78649-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="78649-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="78649-125">identityResourceIdentifier</span></span>|<span data-ttu-id="78649-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="78649-126">String</span></span>|<span data-ttu-id="78649-127">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="78649-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="78649-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="78649-128">identityVersion</span></span>|<span data-ttu-id="78649-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="78649-129">String</span></span>|<span data-ttu-id="78649-130">Die Identität-Version.</span><span class="sxs-lookup"><span data-stu-id="78649-130">The Identity Version.</span></span>|
|<span data-ttu-id="78649-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="78649-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="78649-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="78649-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="78649-133">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="78649-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78649-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="78649-134">Relationships</span></span>
<span data-ttu-id="78649-135">Keine</span><span class="sxs-lookup"><span data-stu-id="78649-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78649-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="78649-136">JSON Representation</span></span>
<span data-ttu-id="78649-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="78649-137">Here is a JSON representation of the resource.</span></span>
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




