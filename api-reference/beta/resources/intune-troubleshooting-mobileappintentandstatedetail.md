---
title: Ressourcentyp mobileAppIntentAndStateDetail
description: Mobile App beabsichtigt und Installationsstatus für ein bestimmtes Gerät.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5ef88a1fa346784ae00a125a487ca844c58d62eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414256"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="3507c-103">Ressourcentyp mobileAppIntentAndStateDetail</span><span class="sxs-lookup"><span data-stu-id="3507c-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="3507c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="3507c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3507c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3507c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3507c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3507c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3507c-107">Mobile App beabsichtigt und Installationsstatus für ein bestimmtes Gerät.</span><span class="sxs-lookup"><span data-stu-id="3507c-107">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="3507c-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3507c-108">Properties</span></span>
|<span data-ttu-id="3507c-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3507c-109">Property</span></span>|<span data-ttu-id="3507c-110">Typ</span><span class="sxs-lookup"><span data-stu-id="3507c-110">Type</span></span>|<span data-ttu-id="3507c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3507c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3507c-112">applicationId</span><span class="sxs-lookup"><span data-stu-id="3507c-112">applicationId</span></span>|<span data-ttu-id="3507c-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3507c-113">String</span></span>|<span data-ttu-id="3507c-114">MobieApp-Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="3507c-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="3507c-115">displayName</span><span class="sxs-lookup"><span data-stu-id="3507c-115">displayName</span></span>|<span data-ttu-id="3507c-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3507c-116">String</span></span>|<span data-ttu-id="3507c-117">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="3507c-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="3507c-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="3507c-118">mobileAppIntent</span></span>|[<span data-ttu-id="3507c-119">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="3507c-119">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="3507c-120">Mobile App beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="3507c-120">Mobile App Intent.</span></span> <span data-ttu-id="3507c-121">Mögliche Werte sind: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment` und `exclude`.</span><span class="sxs-lookup"><span data-stu-id="3507c-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="3507c-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="3507c-122">displayVersion</span></span>|<span data-ttu-id="3507c-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3507c-123">String</span></span>|<span data-ttu-id="3507c-124">Menschen lesbare Version der Anwendung</span><span class="sxs-lookup"><span data-stu-id="3507c-124">Human readable version of the application</span></span>|
|<span data-ttu-id="3507c-125">installState</span><span class="sxs-lookup"><span data-stu-id="3507c-125">installState</span></span>|[<span data-ttu-id="3507c-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="3507c-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="3507c-127">Der Installationsstatus der app.</span><span class="sxs-lookup"><span data-stu-id="3507c-127">The install state of the app.</span></span> <span data-ttu-id="3507c-128">Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="3507c-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="3507c-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="3507c-129">supportedDeviceTypes</span></span>|<span data-ttu-id="3507c-130">[MobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="3507c-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="3507c-131">Die unterstützten Plattformen für die app.</span><span class="sxs-lookup"><span data-stu-id="3507c-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3507c-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3507c-132">Relationships</span></span>
<span data-ttu-id="3507c-133">Keine</span><span class="sxs-lookup"><span data-stu-id="3507c-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3507c-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3507c-134">JSON Representation</span></span>
<span data-ttu-id="3507c-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3507c-135">Here is a JSON representation of the resource.</span></span>
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




