---
title: deviceOperatingSystemSummary-Ressourcentyp
description: Betriebssystemzusammenfassung für das Gerät
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3cf55de11b4d8610cb0622eca9ab740a6b2a40b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157302"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="8e541-103">deviceOperatingSystemSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8e541-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="8e541-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8e541-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e541-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8e541-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e541-106">Betriebssystem des Geräts – Zusammenfassung.</span><span class="sxs-lookup"><span data-stu-id="8e541-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="8e541-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8e541-107">Properties</span></span>
|<span data-ttu-id="8e541-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e541-108">Property</span></span>|<span data-ttu-id="8e541-109">Typ</span><span class="sxs-lookup"><span data-stu-id="8e541-109">Type</span></span>|<span data-ttu-id="8e541-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e541-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e541-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="8e541-111">androidCount</span></span>|<span data-ttu-id="8e541-112">Int32</span><span class="sxs-lookup"><span data-stu-id="8e541-112">Int32</span></span>|<span data-ttu-id="8e541-113">Anzahl der Android-Geräte.</span><span class="sxs-lookup"><span data-stu-id="8e541-113">Number of android device count.</span></span>|
|<span data-ttu-id="8e541-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="8e541-114">iosCount</span></span>|<span data-ttu-id="8e541-115">Int32</span><span class="sxs-lookup"><span data-stu-id="8e541-115">Int32</span></span>|<span data-ttu-id="8e541-116">Anzahl der iOS-Geräte.</span><span class="sxs-lookup"><span data-stu-id="8e541-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="8e541-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="8e541-117">macOSCount</span></span>|<span data-ttu-id="8e541-118">Int32</span><span class="sxs-lookup"><span data-stu-id="8e541-118">Int32</span></span>|<span data-ttu-id="8e541-119">Anzahl der Mac OS X-Geräte.</span><span class="sxs-lookup"><span data-stu-id="8e541-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="8e541-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="8e541-120">windowsMobileCount</span></span>|<span data-ttu-id="8e541-121">Int32</span><span class="sxs-lookup"><span data-stu-id="8e541-121">Int32</span></span>|<span data-ttu-id="8e541-122">Anzahl der Windows Mobile-Geräte.</span><span class="sxs-lookup"><span data-stu-id="8e541-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="8e541-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="8e541-123">windowsCount</span></span>|<span data-ttu-id="8e541-124">Int32</span><span class="sxs-lookup"><span data-stu-id="8e541-124">Int32</span></span>|<span data-ttu-id="8e541-125">Anzahl der Windows-Geräte.</span><span class="sxs-lookup"><span data-stu-id="8e541-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="8e541-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="8e541-126">unknownCount</span></span>|<span data-ttu-id="8e541-127">Int32</span><span class="sxs-lookup"><span data-stu-id="8e541-127">Int32</span></span>|<span data-ttu-id="8e541-128">Anzahl von unbekannten Geräten.</span><span class="sxs-lookup"><span data-stu-id="8e541-128">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e541-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8e541-129">Relationships</span></span>
<span data-ttu-id="8e541-130">Keine</span><span class="sxs-lookup"><span data-stu-id="8e541-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e541-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8e541-131">JSON Representation</span></span>
<span data-ttu-id="8e541-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8e541-132">Here is a JSON representation of the resource.</span></span>
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




