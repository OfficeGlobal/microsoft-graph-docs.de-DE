---
title: Ressourcentyp mobileAppIntentAndStateDetail
description: Mobile App beabsichtigt und Installationsstatus für ein bestimmtes Gerät.
author: tfitzmac
ms.openlocfilehash: 6a0a52d1cf8576778060c6f7b5e337e6e7a115e5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339221"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="e45dd-103">Ressourcentyp mobileAppIntentAndStateDetail</span><span class="sxs-lookup"><span data-stu-id="e45dd-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="e45dd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e45dd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e45dd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e45dd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e45dd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e45dd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e45dd-107">Mobile App beabsichtigt und Installationsstatus für ein bestimmtes Gerät.</span><span class="sxs-lookup"><span data-stu-id="e45dd-107">Mobile App Intent and Install State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="e45dd-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e45dd-108">Properties</span></span>
|<span data-ttu-id="e45dd-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e45dd-109">Property</span></span>|<span data-ttu-id="e45dd-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e45dd-110">Type</span></span>|<span data-ttu-id="e45dd-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e45dd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e45dd-112">applicationId</span><span class="sxs-lookup"><span data-stu-id="e45dd-112">applicationId</span></span>|<span data-ttu-id="e45dd-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e45dd-113">String</span></span>|<span data-ttu-id="e45dd-114">MobieApp-Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="e45dd-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="e45dd-115">displayName</span><span class="sxs-lookup"><span data-stu-id="e45dd-115">displayName</span></span>|<span data-ttu-id="e45dd-116">String</span><span class="sxs-lookup"><span data-stu-id="e45dd-116">String</span></span>|<span data-ttu-id="e45dd-117">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="e45dd-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="e45dd-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="e45dd-118">mobileAppIntent</span></span>|[<span data-ttu-id="e45dd-119">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="e45dd-119">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="e45dd-120">Mobile App beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="e45dd-120">Mobile App Intent.</span></span> <span data-ttu-id="e45dd-121">Mögliche Werte sind: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment` und `exclude`.</span><span class="sxs-lookup"><span data-stu-id="e45dd-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="e45dd-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="e45dd-122">displayVersion</span></span>|<span data-ttu-id="e45dd-123">String</span><span class="sxs-lookup"><span data-stu-id="e45dd-123">String</span></span>|<span data-ttu-id="e45dd-124">Menschen lesbare Version der Anwendung</span><span class="sxs-lookup"><span data-stu-id="e45dd-124">Human readable version of the application</span></span>|
|<span data-ttu-id="e45dd-125">installState</span><span class="sxs-lookup"><span data-stu-id="e45dd-125">installState</span></span>|[<span data-ttu-id="e45dd-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="e45dd-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="e45dd-127">Der Installationsstatus der app.</span><span class="sxs-lookup"><span data-stu-id="e45dd-127">The install state of the app.</span></span> <span data-ttu-id="e45dd-128">Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="e45dd-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="e45dd-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="e45dd-129">supportedDeviceTypes</span></span>|<span data-ttu-id="e45dd-130">[MobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e45dd-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="e45dd-131">Die unterstützten Plattformen für die app.</span><span class="sxs-lookup"><span data-stu-id="e45dd-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e45dd-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e45dd-132">Relationships</span></span>
<span data-ttu-id="e45dd-133">Keine</span><span class="sxs-lookup"><span data-stu-id="e45dd-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e45dd-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e45dd-134">JSON Representation</span></span>
<span data-ttu-id="e45dd-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e45dd-135">Here is a JSON representation of the resource.</span></span>
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





