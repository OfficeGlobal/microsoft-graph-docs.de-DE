---
title: deviceOperatingSystemSummary-Ressourcentyp
description: Betriebssystemzusammenfassung für das Gerät
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53c806e250d6b201e6dfe49d90685c4144913182
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250404"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="4c0ba-103">deviceOperatingSystemSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4c0ba-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="4c0ba-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4c0ba-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c0ba-105">Betriebssystem des Geräts – Zusammenfassung.</span><span class="sxs-lookup"><span data-stu-id="4c0ba-105">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="4c0ba-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4c0ba-106">Properties</span></span>
|<span data-ttu-id="4c0ba-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4c0ba-107">Property</span></span>|<span data-ttu-id="4c0ba-108">Typ</span><span class="sxs-lookup"><span data-stu-id="4c0ba-108">Type</span></span>|<span data-ttu-id="4c0ba-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c0ba-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c0ba-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="4c0ba-110">androidCount</span></span>|<span data-ttu-id="4c0ba-111">Int32</span><span class="sxs-lookup"><span data-stu-id="4c0ba-111">Int32</span></span>|<span data-ttu-id="4c0ba-112">Anzahl der Android-Geräte.</span><span class="sxs-lookup"><span data-stu-id="4c0ba-112">Number of android device count.</span></span>|
|<span data-ttu-id="4c0ba-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="4c0ba-113">iosCount</span></span>|<span data-ttu-id="4c0ba-114">Int32</span><span class="sxs-lookup"><span data-stu-id="4c0ba-114">Int32</span></span>|<span data-ttu-id="4c0ba-115">Anzahl der iOS-Geräte.</span><span class="sxs-lookup"><span data-stu-id="4c0ba-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="4c0ba-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="4c0ba-116">macOSCount</span></span>|<span data-ttu-id="4c0ba-117">Int32</span><span class="sxs-lookup"><span data-stu-id="4c0ba-117">Int32</span></span>|<span data-ttu-id="4c0ba-118">Anzahl der Mac OS X-Geräte.</span><span class="sxs-lookup"><span data-stu-id="4c0ba-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="4c0ba-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="4c0ba-119">windowsMobileCount</span></span>|<span data-ttu-id="4c0ba-120">Int32</span><span class="sxs-lookup"><span data-stu-id="4c0ba-120">Int32</span></span>|<span data-ttu-id="4c0ba-121">Anzahl der Windows Mobile-Geräte.</span><span class="sxs-lookup"><span data-stu-id="4c0ba-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="4c0ba-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="4c0ba-122">windowsCount</span></span>|<span data-ttu-id="4c0ba-123">Int32</span><span class="sxs-lookup"><span data-stu-id="4c0ba-123">Int32</span></span>|<span data-ttu-id="4c0ba-124">Anzahl der Windows-Geräte.</span><span class="sxs-lookup"><span data-stu-id="4c0ba-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="4c0ba-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="4c0ba-125">unknownCount</span></span>|<span data-ttu-id="4c0ba-126">Int32</span><span class="sxs-lookup"><span data-stu-id="4c0ba-126">Int32</span></span>|<span data-ttu-id="4c0ba-127">Anzahl von unbekannten Geräten.</span><span class="sxs-lookup"><span data-stu-id="4c0ba-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c0ba-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4c0ba-128">Relationships</span></span>
<span data-ttu-id="4c0ba-129">Keine</span><span class="sxs-lookup"><span data-stu-id="4c0ba-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c0ba-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4c0ba-130">JSON Representation</span></span>
<span data-ttu-id="4c0ba-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4c0ba-131">Here is a JSON representation of the resource.</span></span>
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



