---
title: deviceOperatingSystemSummary-Ressourcentyp
description: Betriebssystemzusammenfassung für das Gerät
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 009998d495eb033510bbc27437b72f866fd4ed7e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410770"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="bb558-103">deviceOperatingSystemSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bb558-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="bb558-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="bb558-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bb558-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bb558-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb558-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bb558-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb558-107">Betriebssystem des Geräts – Zusammenfassung.</span><span class="sxs-lookup"><span data-stu-id="bb558-107">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="bb558-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bb558-108">Properties</span></span>
|<span data-ttu-id="bb558-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bb558-109">Property</span></span>|<span data-ttu-id="bb558-110">Typ</span><span class="sxs-lookup"><span data-stu-id="bb558-110">Type</span></span>|<span data-ttu-id="bb558-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb558-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb558-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="bb558-112">androidCount</span></span>|<span data-ttu-id="bb558-113">Int32</span><span class="sxs-lookup"><span data-stu-id="bb558-113">Int32</span></span>|<span data-ttu-id="bb558-114">Anzahl der Android-Geräte.</span><span class="sxs-lookup"><span data-stu-id="bb558-114">Number of android device count.</span></span>|
|<span data-ttu-id="bb558-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="bb558-115">iosCount</span></span>|<span data-ttu-id="bb558-116">Int32</span><span class="sxs-lookup"><span data-stu-id="bb558-116">Int32</span></span>|<span data-ttu-id="bb558-117">Anzahl der iOS-Geräte.</span><span class="sxs-lookup"><span data-stu-id="bb558-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="bb558-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="bb558-118">macOSCount</span></span>|<span data-ttu-id="bb558-119">Int32</span><span class="sxs-lookup"><span data-stu-id="bb558-119">Int32</span></span>|<span data-ttu-id="bb558-120">Anzahl der Mac OS X-Geräte.</span><span class="sxs-lookup"><span data-stu-id="bb558-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="bb558-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="bb558-121">windowsMobileCount</span></span>|<span data-ttu-id="bb558-122">Int32</span><span class="sxs-lookup"><span data-stu-id="bb558-122">Int32</span></span>|<span data-ttu-id="bb558-123">Anzahl der Windows Mobile-Geräte.</span><span class="sxs-lookup"><span data-stu-id="bb558-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="bb558-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="bb558-124">windowsCount</span></span>|<span data-ttu-id="bb558-125">Int32</span><span class="sxs-lookup"><span data-stu-id="bb558-125">Int32</span></span>|<span data-ttu-id="bb558-126">Anzahl der Windows-Geräte.</span><span class="sxs-lookup"><span data-stu-id="bb558-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="bb558-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="bb558-127">unknownCount</span></span>|<span data-ttu-id="bb558-128">Int32</span><span class="sxs-lookup"><span data-stu-id="bb558-128">Int32</span></span>|<span data-ttu-id="bb558-129">Anzahl von unbekannten Geräten.</span><span class="sxs-lookup"><span data-stu-id="bb558-129">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb558-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bb558-130">Relationships</span></span>
<span data-ttu-id="bb558-131">Keine</span><span class="sxs-lookup"><span data-stu-id="bb558-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb558-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bb558-132">JSON Representation</span></span>
<span data-ttu-id="bb558-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bb558-133">Here is a JSON representation of the resource.</span></span>
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




