---
title: Ressourcentyp mobileAppIntentAndStateDetail
description: Mobile App beabsichtigt und Installationsstatus für ein bestimmtes Gerät.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ad20ef00cbc8e5295a96107fbce2f5e7f1cb978a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805810"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="30157-103">Ressourcentyp mobileAppIntentAndStateDetail</span><span class="sxs-lookup"><span data-stu-id="30157-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="30157-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="30157-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30157-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="30157-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30157-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="30157-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30157-107">Mobile App beabsichtigt und Installationsstatus für ein bestimmtes Gerät.</span><span class="sxs-lookup"><span data-stu-id="30157-107">Mobile App Intent and Install State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="30157-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="30157-108">Properties</span></span>
|<span data-ttu-id="30157-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="30157-109">Property</span></span>|<span data-ttu-id="30157-110">Typ</span><span class="sxs-lookup"><span data-stu-id="30157-110">Type</span></span>|<span data-ttu-id="30157-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30157-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30157-112">applicationId</span><span class="sxs-lookup"><span data-stu-id="30157-112">applicationId</span></span>|<span data-ttu-id="30157-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="30157-113">String</span></span>|<span data-ttu-id="30157-114">MobieApp-Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="30157-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="30157-115">displayName</span><span class="sxs-lookup"><span data-stu-id="30157-115">displayName</span></span>|<span data-ttu-id="30157-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="30157-116">String</span></span>|<span data-ttu-id="30157-117">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="30157-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="30157-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="30157-118">mobileAppIntent</span></span>|[<span data-ttu-id="30157-119">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="30157-119">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="30157-120">Mobile App beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="30157-120">Mobile App Intent.</span></span> <span data-ttu-id="30157-121">Mögliche Werte sind: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment` und `exclude`.</span><span class="sxs-lookup"><span data-stu-id="30157-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="30157-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="30157-122">displayVersion</span></span>|<span data-ttu-id="30157-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="30157-123">String</span></span>|<span data-ttu-id="30157-124">Menschen lesbare Version der Anwendung</span><span class="sxs-lookup"><span data-stu-id="30157-124">Human readable version of the application</span></span>|
|<span data-ttu-id="30157-125">installState</span><span class="sxs-lookup"><span data-stu-id="30157-125">installState</span></span>|[<span data-ttu-id="30157-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="30157-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="30157-127">Der Installationsstatus der app.</span><span class="sxs-lookup"><span data-stu-id="30157-127">The install state of the app.</span></span> <span data-ttu-id="30157-128">Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="30157-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="30157-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="30157-129">supportedDeviceTypes</span></span>|<span data-ttu-id="30157-130">[MobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="30157-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="30157-131">Die unterstützten Plattformen für die app.</span><span class="sxs-lookup"><span data-stu-id="30157-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30157-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="30157-132">Relationships</span></span>
<span data-ttu-id="30157-133">Keine</span><span class="sxs-lookup"><span data-stu-id="30157-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="30157-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="30157-134">JSON Representation</span></span>
<span data-ttu-id="30157-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="30157-135">Here is a JSON representation of the resource.</span></span>
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





