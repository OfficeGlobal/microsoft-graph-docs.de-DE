---
title: deviceEnrollmentPlatformRestriction-Ressourcentyp
description: Plattformspezifische Registrierungseinschränkungen
ms.openlocfilehash: b6d4ea3acf4995548fce7f2c86b3c95c444b59b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020041"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="14701-103">deviceEnrollmentPlatformRestriction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="14701-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="14701-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="14701-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14701-105">Plattformspezifische Registrierungseinschränkungen</span><span class="sxs-lookup"><span data-stu-id="14701-105">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="14701-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="14701-106">Properties</span></span>
|<span data-ttu-id="14701-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="14701-107">Property</span></span>|<span data-ttu-id="14701-108">Typ</span><span class="sxs-lookup"><span data-stu-id="14701-108">Type</span></span>|<span data-ttu-id="14701-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14701-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14701-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="14701-110">platformBlocked</span></span>|<span data-ttu-id="14701-111">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="14701-111">Boolean</span></span>|<span data-ttu-id="14701-112">Sperren der Plattform für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="14701-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="14701-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="14701-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="14701-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="14701-114">Boolean</span></span>|<span data-ttu-id="14701-115">Sperren privat genutzter Geräte für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="14701-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="14701-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="14701-116">osMinimumVersion</span></span>|<span data-ttu-id="14701-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="14701-117">String</span></span>|<span data-ttu-id="14701-118">Unterstützte mindestens benötigte iOS-Version</span><span class="sxs-lookup"><span data-stu-id="14701-118">Min OS version supported</span></span>|
|<span data-ttu-id="14701-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="14701-119">osMaximumVersion</span></span>|<span data-ttu-id="14701-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="14701-120">String</span></span>|<span data-ttu-id="14701-121">Unterstützte maximal verwendbare iOS-Version</span><span class="sxs-lookup"><span data-stu-id="14701-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="14701-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="14701-122">Relationships</span></span>
<span data-ttu-id="14701-123">Keine</span><span class="sxs-lookup"><span data-stu-id="14701-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="14701-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="14701-124">JSON Representation</span></span>
<span data-ttu-id="14701-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="14701-125">Here is a JSON representation of the resource.</span></span>
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



