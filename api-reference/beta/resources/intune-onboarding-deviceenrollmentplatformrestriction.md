---
title: deviceEnrollmentPlatformRestriction-Ressourcentyp
description: Plattformspezifische Registrierungseinschränkungen
author: tfitzmac
ms.openlocfilehash: 22401c83b3e68d66a2bd7a39359602e2aca0a932
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304123"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="5feb3-103">deviceEnrollmentPlatformRestriction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5feb3-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="5feb3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5feb3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5feb3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5feb3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5feb3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5feb3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5feb3-107">Plattformspezifische Registrierungseinschränkungen</span><span class="sxs-lookup"><span data-stu-id="5feb3-107">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="5feb3-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5feb3-108">Properties</span></span>
|<span data-ttu-id="5feb3-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5feb3-109">Property</span></span>|<span data-ttu-id="5feb3-110">Typ</span><span class="sxs-lookup"><span data-stu-id="5feb3-110">Type</span></span>|<span data-ttu-id="5feb3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5feb3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5feb3-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="5feb3-112">platformBlocked</span></span>|<span data-ttu-id="5feb3-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5feb3-113">Boolean</span></span>|<span data-ttu-id="5feb3-114">Sperren der Plattform für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="5feb3-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="5feb3-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="5feb3-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="5feb3-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5feb3-116">Boolean</span></span>|<span data-ttu-id="5feb3-117">Sperren privat genutzter Geräte für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="5feb3-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="5feb3-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5feb3-118">osMinimumVersion</span></span>|<span data-ttu-id="5feb3-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5feb3-119">String</span></span>|<span data-ttu-id="5feb3-120">Unterstützte mindestens benötigte iOS-Version</span><span class="sxs-lookup"><span data-stu-id="5feb3-120">Min OS version supported</span></span>|
|<span data-ttu-id="5feb3-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5feb3-121">osMaximumVersion</span></span>|<span data-ttu-id="5feb3-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5feb3-122">String</span></span>|<span data-ttu-id="5feb3-123">Unterstützte maximal verwendbare iOS-Version</span><span class="sxs-lookup"><span data-stu-id="5feb3-123">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="5feb3-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5feb3-124">Relationships</span></span>
<span data-ttu-id="5feb3-125">Keine</span><span class="sxs-lookup"><span data-stu-id="5feb3-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5feb3-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5feb3-126">JSON Representation</span></span>
<span data-ttu-id="5feb3-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5feb3-127">Here is a JSON representation of the resource.</span></span>
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





