---
title: deviceOperatingSystemSummary-Ressourcentyp
description: Betriebssystemzusammenfassung für das Gerät
ms.openlocfilehash: 1a543f21d1f82b9f2bee0f004d3b8fab88c863b0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018304"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="07dcb-103">deviceOperatingSystemSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="07dcb-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="07dcb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="07dcb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07dcb-105">Betriebssystem des Geräts – Zusammenfassung.</span><span class="sxs-lookup"><span data-stu-id="07dcb-105">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="07dcb-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="07dcb-106">Properties</span></span>
|<span data-ttu-id="07dcb-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="07dcb-107">Property</span></span>|<span data-ttu-id="07dcb-108">Typ</span><span class="sxs-lookup"><span data-stu-id="07dcb-108">Type</span></span>|<span data-ttu-id="07dcb-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07dcb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07dcb-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="07dcb-110">androidCount</span></span>|<span data-ttu-id="07dcb-111">Int32</span><span class="sxs-lookup"><span data-stu-id="07dcb-111">Int32</span></span>|<span data-ttu-id="07dcb-112">Anzahl der Android-Geräte.</span><span class="sxs-lookup"><span data-stu-id="07dcb-112">Number of android device count.</span></span>|
|<span data-ttu-id="07dcb-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="07dcb-113">iosCount</span></span>|<span data-ttu-id="07dcb-114">Int32</span><span class="sxs-lookup"><span data-stu-id="07dcb-114">Int32</span></span>|<span data-ttu-id="07dcb-115">Anzahl der iOS-Geräte.</span><span class="sxs-lookup"><span data-stu-id="07dcb-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="07dcb-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="07dcb-116">macOSCount</span></span>|<span data-ttu-id="07dcb-117">Int32</span><span class="sxs-lookup"><span data-stu-id="07dcb-117">Int32</span></span>|<span data-ttu-id="07dcb-118">Anzahl der Mac OS X-Geräte.</span><span class="sxs-lookup"><span data-stu-id="07dcb-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="07dcb-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="07dcb-119">windowsMobileCount</span></span>|<span data-ttu-id="07dcb-120">Int32</span><span class="sxs-lookup"><span data-stu-id="07dcb-120">Int32</span></span>|<span data-ttu-id="07dcb-121">Anzahl der Windows Mobile-Geräte.</span><span class="sxs-lookup"><span data-stu-id="07dcb-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="07dcb-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="07dcb-122">windowsCount</span></span>|<span data-ttu-id="07dcb-123">Int32</span><span class="sxs-lookup"><span data-stu-id="07dcb-123">Int32</span></span>|<span data-ttu-id="07dcb-124">Anzahl der Windows-Geräte.</span><span class="sxs-lookup"><span data-stu-id="07dcb-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="07dcb-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="07dcb-125">unknownCount</span></span>|<span data-ttu-id="07dcb-126">Int32</span><span class="sxs-lookup"><span data-stu-id="07dcb-126">Int32</span></span>|<span data-ttu-id="07dcb-127">Anzahl von unbekannten Geräten.</span><span class="sxs-lookup"><span data-stu-id="07dcb-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07dcb-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="07dcb-128">Relationships</span></span>
<span data-ttu-id="07dcb-129">Keine</span><span class="sxs-lookup"><span data-stu-id="07dcb-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="07dcb-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="07dcb-130">JSON Representation</span></span>
<span data-ttu-id="07dcb-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="07dcb-131">Here is a JSON representation of the resource.</span></span>
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



