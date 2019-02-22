---
title: mobileAppIntentAndStateDetail-Ressourcentyp
description: Ziel für Mobile Apps und Installationsstatus für ein bestimmtes Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76db364b53c9ccb6b4057835b853705cd49ca410
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146753"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="427e9-103">mobileAppIntentAndStateDetail-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="427e9-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="427e9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="427e9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="427e9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="427e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="427e9-106">Ziel für Mobile Apps und Installationsstatus für ein bestimmtes Gerät.</span><span class="sxs-lookup"><span data-stu-id="427e9-106">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="427e9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="427e9-107">Properties</span></span>
|<span data-ttu-id="427e9-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="427e9-108">Property</span></span>|<span data-ttu-id="427e9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="427e9-109">Type</span></span>|<span data-ttu-id="427e9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="427e9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="427e9-111">applicationId</span><span class="sxs-lookup"><span data-stu-id="427e9-111">applicationId</span></span>|<span data-ttu-id="427e9-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="427e9-112">String</span></span>|<span data-ttu-id="427e9-113">MobieApp-Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="427e9-113">MobieApp identifier.</span></span>|
|<span data-ttu-id="427e9-114">displayName</span><span class="sxs-lookup"><span data-stu-id="427e9-114">displayName</span></span>|<span data-ttu-id="427e9-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="427e9-115">String</span></span>|<span data-ttu-id="427e9-116">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="427e9-116">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="427e9-117">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="427e9-117">mobileAppIntent</span></span>|[<span data-ttu-id="427e9-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="427e9-118">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="427e9-119">Mobile App-Absicht.</span><span class="sxs-lookup"><span data-stu-id="427e9-119">Mobile App Intent.</span></span> <span data-ttu-id="427e9-120">Mögliche Werte sind: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment` und `exclude`.</span><span class="sxs-lookup"><span data-stu-id="427e9-120">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="427e9-121">Display Version</span><span class="sxs-lookup"><span data-stu-id="427e9-121">displayVersion</span></span>|<span data-ttu-id="427e9-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="427e9-122">String</span></span>|<span data-ttu-id="427e9-123">Lesbare Version der Anwendung</span><span class="sxs-lookup"><span data-stu-id="427e9-123">Human readable version of the application</span></span>|
|<span data-ttu-id="427e9-124">installState</span><span class="sxs-lookup"><span data-stu-id="427e9-124">installState</span></span>|[<span data-ttu-id="427e9-125">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="427e9-125">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="427e9-126">Der Installationsstatus der app.</span><span class="sxs-lookup"><span data-stu-id="427e9-126">The install state of the app.</span></span> <span data-ttu-id="427e9-127">Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="427e9-127">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="427e9-128">Mobileappintentandstatedetail</span><span class="sxs-lookup"><span data-stu-id="427e9-128">supportedDeviceTypes</span></span>|<span data-ttu-id="427e9-129">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="427e9-129">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="427e9-130">Die unterstützten Plattformen für die app.</span><span class="sxs-lookup"><span data-stu-id="427e9-130">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="427e9-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="427e9-131">Relationships</span></span>
<span data-ttu-id="427e9-132">Keine</span><span class="sxs-lookup"><span data-stu-id="427e9-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="427e9-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="427e9-133">JSON Representation</span></span>
<span data-ttu-id="427e9-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="427e9-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndStateDetail",
  "applicationId": "String",
  "displayName": "String",
  "mobileAppIntent": "String",
  "displayVersion": "String",
  "installState": "String",
  "supportedDeviceTypes": [
    {
      "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
      "type": "String",
      "minimumOperatingSystemVersion": "String",
      "maximumOperatingSystemVersion": "String"
    }
  ]
}
```




