---
title: deviceEnrollmentPlatformRestriction-Ressourcentyp
description: Plattformspezifische Registrierungseinschränkungen
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e5189b286de61375715944c5ac979d847392a18c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917762"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="07119-103">deviceEnrollmentPlatformRestriction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="07119-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="07119-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="07119-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07119-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="07119-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07119-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="07119-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07119-107">Plattformspezifische Registrierungseinschränkungen</span><span class="sxs-lookup"><span data-stu-id="07119-107">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="07119-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="07119-108">Properties</span></span>
|<span data-ttu-id="07119-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="07119-109">Property</span></span>|<span data-ttu-id="07119-110">Typ</span><span class="sxs-lookup"><span data-stu-id="07119-110">Type</span></span>|<span data-ttu-id="07119-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07119-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07119-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="07119-112">platformBlocked</span></span>|<span data-ttu-id="07119-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="07119-113">Boolean</span></span>|<span data-ttu-id="07119-114">Sperren der Plattform für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="07119-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="07119-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="07119-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="07119-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="07119-116">Boolean</span></span>|<span data-ttu-id="07119-117">Sperren privat genutzter Geräte für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="07119-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="07119-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="07119-118">osMinimumVersion</span></span>|<span data-ttu-id="07119-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07119-119">String</span></span>|<span data-ttu-id="07119-120">Unterstützte mindestens benötigte iOS-Version</span><span class="sxs-lookup"><span data-stu-id="07119-120">Min OS version supported</span></span>|
|<span data-ttu-id="07119-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="07119-121">osMaximumVersion</span></span>|<span data-ttu-id="07119-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07119-122">String</span></span>|<span data-ttu-id="07119-123">Unterstützte maximal verwendbare iOS-Version</span><span class="sxs-lookup"><span data-stu-id="07119-123">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="07119-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="07119-124">Relationships</span></span>
<span data-ttu-id="07119-125">Keine</span><span class="sxs-lookup"><span data-stu-id="07119-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="07119-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="07119-126">JSON Representation</span></span>
<span data-ttu-id="07119-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="07119-127">Here is a JSON representation of the resource.</span></span>
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





