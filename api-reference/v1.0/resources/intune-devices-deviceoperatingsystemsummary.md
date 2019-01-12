---
title: deviceOperatingSystemSummary-Ressourcentyp
description: Betriebssystemzusammenfassung für das Gerät
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2147034c060fa15e8e799d5ddbe72aabe635af08
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975645"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="f739e-103">deviceOperatingSystemSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f739e-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="f739e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f739e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f739e-105">Betriebssystem des Geräts – Zusammenfassung.</span><span class="sxs-lookup"><span data-stu-id="f739e-105">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="f739e-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f739e-106">Properties</span></span>
|<span data-ttu-id="f739e-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f739e-107">Property</span></span>|<span data-ttu-id="f739e-108">Typ</span><span class="sxs-lookup"><span data-stu-id="f739e-108">Type</span></span>|<span data-ttu-id="f739e-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f739e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f739e-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="f739e-110">androidCount</span></span>|<span data-ttu-id="f739e-111">Int32</span><span class="sxs-lookup"><span data-stu-id="f739e-111">Int32</span></span>|<span data-ttu-id="f739e-112">Anzahl der Android-Geräte.</span><span class="sxs-lookup"><span data-stu-id="f739e-112">Number of android device count.</span></span>|
|<span data-ttu-id="f739e-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="f739e-113">iosCount</span></span>|<span data-ttu-id="f739e-114">Int32</span><span class="sxs-lookup"><span data-stu-id="f739e-114">Int32</span></span>|<span data-ttu-id="f739e-115">Anzahl der iOS-Geräte.</span><span class="sxs-lookup"><span data-stu-id="f739e-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="f739e-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="f739e-116">macOSCount</span></span>|<span data-ttu-id="f739e-117">Int32</span><span class="sxs-lookup"><span data-stu-id="f739e-117">Int32</span></span>|<span data-ttu-id="f739e-118">Anzahl der Mac OS X-Geräte.</span><span class="sxs-lookup"><span data-stu-id="f739e-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="f739e-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="f739e-119">windowsMobileCount</span></span>|<span data-ttu-id="f739e-120">Int32</span><span class="sxs-lookup"><span data-stu-id="f739e-120">Int32</span></span>|<span data-ttu-id="f739e-121">Anzahl der Windows Mobile-Geräte.</span><span class="sxs-lookup"><span data-stu-id="f739e-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="f739e-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="f739e-122">windowsCount</span></span>|<span data-ttu-id="f739e-123">Int32</span><span class="sxs-lookup"><span data-stu-id="f739e-123">Int32</span></span>|<span data-ttu-id="f739e-124">Anzahl der Windows-Geräte.</span><span class="sxs-lookup"><span data-stu-id="f739e-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="f739e-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="f739e-125">unknownCount</span></span>|<span data-ttu-id="f739e-126">Int32</span><span class="sxs-lookup"><span data-stu-id="f739e-126">Int32</span></span>|<span data-ttu-id="f739e-127">Anzahl von unbekannten Geräten.</span><span class="sxs-lookup"><span data-stu-id="f739e-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f739e-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f739e-128">Relationships</span></span>
<span data-ttu-id="f739e-129">Keine</span><span class="sxs-lookup"><span data-stu-id="f739e-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f739e-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f739e-130">JSON Representation</span></span>
<span data-ttu-id="f739e-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f739e-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```



