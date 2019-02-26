---
title: deviceEnrollmentPlatformRestriction-Ressourcentyp
description: Plattformspezifische Registrierungseinschränkungen
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 306f280928c843b596c57e7bdab454fd138851cc
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260837"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="d0d78-103">deviceEnrollmentPlatformRestriction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d0d78-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="d0d78-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d0d78-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0d78-105">Plattformspezifische Registrierungseinschränkungen</span><span class="sxs-lookup"><span data-stu-id="d0d78-105">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="d0d78-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d0d78-106">Properties</span></span>
|<span data-ttu-id="d0d78-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d0d78-107">Property</span></span>|<span data-ttu-id="d0d78-108">Typ</span><span class="sxs-lookup"><span data-stu-id="d0d78-108">Type</span></span>|<span data-ttu-id="d0d78-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0d78-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0d78-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="d0d78-110">platformBlocked</span></span>|<span data-ttu-id="d0d78-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0d78-111">Boolean</span></span>|<span data-ttu-id="d0d78-112">Sperren der Plattform für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="d0d78-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="d0d78-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="d0d78-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="d0d78-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d0d78-114">Boolean</span></span>|<span data-ttu-id="d0d78-115">Sperren privat genutzter Geräte für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="d0d78-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="d0d78-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="d0d78-116">osMinimumVersion</span></span>|<span data-ttu-id="d0d78-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d0d78-117">String</span></span>|<span data-ttu-id="d0d78-118">Unterstützte mindestens benötigte iOS-Version</span><span class="sxs-lookup"><span data-stu-id="d0d78-118">Min OS version supported</span></span>|
|<span data-ttu-id="d0d78-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="d0d78-119">osMaximumVersion</span></span>|<span data-ttu-id="d0d78-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d0d78-120">String</span></span>|<span data-ttu-id="d0d78-121">Unterstützte maximal verwendbare iOS-Version</span><span class="sxs-lookup"><span data-stu-id="d0d78-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0d78-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d0d78-122">Relationships</span></span>
<span data-ttu-id="d0d78-123">Keine</span><span class="sxs-lookup"><span data-stu-id="d0d78-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0d78-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d0d78-124">JSON Representation</span></span>
<span data-ttu-id="d0d78-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d0d78-125">Here is a JSON representation of the resource.</span></span>
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



