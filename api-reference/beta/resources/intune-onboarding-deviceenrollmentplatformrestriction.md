---
title: deviceEnrollmentPlatformRestriction-Ressourcentyp
description: Plattformspezifische Registrierungseinschränkungen
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0bf4748d8dc083fe03b55b5ee88062ebb429f639
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422859"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="0f6f0-103">deviceEnrollmentPlatformRestriction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0f6f0-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="0f6f0-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0f6f0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0f6f0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0f6f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f6f0-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0f6f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f6f0-107">Plattformspezifische Registrierungseinschränkungen</span><span class="sxs-lookup"><span data-stu-id="0f6f0-107">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="0f6f0-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0f6f0-108">Properties</span></span>
|<span data-ttu-id="0f6f0-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f6f0-109">Property</span></span>|<span data-ttu-id="0f6f0-110">Typ</span><span class="sxs-lookup"><span data-stu-id="0f6f0-110">Type</span></span>|<span data-ttu-id="0f6f0-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f6f0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f6f0-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="0f6f0-112">platformBlocked</span></span>|<span data-ttu-id="0f6f0-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0f6f0-113">Boolean</span></span>|<span data-ttu-id="0f6f0-114">Sperren der Plattform für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="0f6f0-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="0f6f0-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="0f6f0-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="0f6f0-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0f6f0-116">Boolean</span></span>|<span data-ttu-id="0f6f0-117">Sperren privat genutzter Geräte für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="0f6f0-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="0f6f0-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0f6f0-118">osMinimumVersion</span></span>|<span data-ttu-id="0f6f0-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0f6f0-119">String</span></span>|<span data-ttu-id="0f6f0-120">Unterstützte mindestens benötigte iOS-Version</span><span class="sxs-lookup"><span data-stu-id="0f6f0-120">Min OS version supported</span></span>|
|<span data-ttu-id="0f6f0-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0f6f0-121">osMaximumVersion</span></span>|<span data-ttu-id="0f6f0-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0f6f0-122">String</span></span>|<span data-ttu-id="0f6f0-123">Unterstützte maximal verwendbare iOS-Version</span><span class="sxs-lookup"><span data-stu-id="0f6f0-123">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f6f0-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0f6f0-124">Relationships</span></span>
<span data-ttu-id="0f6f0-125">Keine</span><span class="sxs-lookup"><span data-stu-id="0f6f0-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f6f0-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0f6f0-126">JSON Representation</span></span>
<span data-ttu-id="0f6f0-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0f6f0-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```




