---
title: deviceEnrollmentPlatformRestriction-Ressourcentyp
description: Plattformspezifische Registrierungseinschränkungen
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eecbc405fd56d21f7be1c7b9bccd5254db89c8d1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140600"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="ccf0f-103">deviceEnrollmentPlatformRestriction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ccf0f-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="ccf0f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ccf0f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccf0f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ccf0f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccf0f-106">Plattformspezifische Registrierungseinschränkungen</span><span class="sxs-lookup"><span data-stu-id="ccf0f-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="ccf0f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ccf0f-107">Properties</span></span>
|<span data-ttu-id="ccf0f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ccf0f-108">Property</span></span>|<span data-ttu-id="ccf0f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ccf0f-109">Type</span></span>|<span data-ttu-id="ccf0f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ccf0f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccf0f-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="ccf0f-111">platformBlocked</span></span>|<span data-ttu-id="ccf0f-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccf0f-112">Boolean</span></span>|<span data-ttu-id="ccf0f-113">Sperren der Plattform für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="ccf0f-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="ccf0f-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="ccf0f-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="ccf0f-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ccf0f-115">Boolean</span></span>|<span data-ttu-id="ccf0f-116">Sperren privat genutzter Geräte für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="ccf0f-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="ccf0f-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ccf0f-117">osMinimumVersion</span></span>|<span data-ttu-id="ccf0f-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ccf0f-118">String</span></span>|<span data-ttu-id="ccf0f-119">Unterstützte mindestens benötigte iOS-Version</span><span class="sxs-lookup"><span data-stu-id="ccf0f-119">Min OS version supported</span></span>|
|<span data-ttu-id="ccf0f-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ccf0f-120">osMaximumVersion</span></span>|<span data-ttu-id="ccf0f-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ccf0f-121">String</span></span>|<span data-ttu-id="ccf0f-122">Unterstützte maximal verwendbare iOS-Version</span><span class="sxs-lookup"><span data-stu-id="ccf0f-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccf0f-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ccf0f-123">Relationships</span></span>
<span data-ttu-id="ccf0f-124">Keine</span><span class="sxs-lookup"><span data-stu-id="ccf0f-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ccf0f-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ccf0f-125">JSON Representation</span></span>
<span data-ttu-id="ccf0f-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ccf0f-126">Here is a JSON representation of the resource.</span></span>
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




