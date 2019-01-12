---
title: deviceEnrollmentPlatformRestriction-Ressourcentyp
description: Plattformspezifische Registrierungseinschränkungen
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7879b7f6585908aa760c3169e950cc5257bf49a7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929067"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="084f4-103">deviceEnrollmentPlatformRestriction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="084f4-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="084f4-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="084f4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="084f4-105">Plattformspezifische Registrierungseinschränkungen</span><span class="sxs-lookup"><span data-stu-id="084f4-105">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="084f4-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="084f4-106">Properties</span></span>
|<span data-ttu-id="084f4-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="084f4-107">Property</span></span>|<span data-ttu-id="084f4-108">Typ</span><span class="sxs-lookup"><span data-stu-id="084f4-108">Type</span></span>|<span data-ttu-id="084f4-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="084f4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="084f4-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="084f4-110">platformBlocked</span></span>|<span data-ttu-id="084f4-111">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="084f4-111">Boolean</span></span>|<span data-ttu-id="084f4-112">Sperren der Plattform für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="084f4-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="084f4-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="084f4-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="084f4-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="084f4-114">Boolean</span></span>|<span data-ttu-id="084f4-115">Sperren privat genutzter Geräte für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="084f4-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="084f4-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="084f4-116">osMinimumVersion</span></span>|<span data-ttu-id="084f4-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="084f4-117">String</span></span>|<span data-ttu-id="084f4-118">Unterstützte mindestens benötigte iOS-Version</span><span class="sxs-lookup"><span data-stu-id="084f4-118">Min OS version supported</span></span>|
|<span data-ttu-id="084f4-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="084f4-119">osMaximumVersion</span></span>|<span data-ttu-id="084f4-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="084f4-120">String</span></span>|<span data-ttu-id="084f4-121">Unterstützte maximal verwendbare iOS-Version</span><span class="sxs-lookup"><span data-stu-id="084f4-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="084f4-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="084f4-122">Relationships</span></span>
<span data-ttu-id="084f4-123">Keine</span><span class="sxs-lookup"><span data-stu-id="084f4-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="084f4-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="084f4-124">JSON Representation</span></span>
<span data-ttu-id="084f4-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="084f4-125">Here is a JSON representation of the resource.</span></span>
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



