---
title: Ressourcentyp excludedApps
description: Enthält Eigenschaften für die ausgeschlossenen Office365 Apps.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1d3cd9a159597689a64070181640415a6ce2fc61
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395678"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="fd288-103">Ressourcentyp excludedApps</span><span class="sxs-lookup"><span data-stu-id="fd288-103">excludedApps resource type</span></span>

> <span data-ttu-id="fd288-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="fd288-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fd288-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fd288-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd288-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fd288-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd288-107">Enthält Eigenschaften für die ausgeschlossenen Office365 Apps.</span><span class="sxs-lookup"><span data-stu-id="fd288-107">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="fd288-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fd288-108">Properties</span></span>
|<span data-ttu-id="fd288-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fd288-109">Property</span></span>|<span data-ttu-id="fd288-110">Typ</span><span class="sxs-lookup"><span data-stu-id="fd288-110">Type</span></span>|<span data-ttu-id="fd288-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd288-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd288-112">access</span><span class="sxs-lookup"><span data-stu-id="fd288-112">access</span></span>|<span data-ttu-id="fd288-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd288-113">Boolean</span></span>|<span data-ttu-id="fd288-114">Der Wert für die If MS Office Access davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="fd288-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="fd288-115">Excel-</span><span class="sxs-lookup"><span data-stu-id="fd288-115">excel</span></span>|<span data-ttu-id="fd288-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd288-116">Boolean</span></span>|<span data-ttu-id="fd288-117">Der Wert für die If MS Office Excel davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="fd288-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="fd288-118">Groove</span><span class="sxs-lookup"><span data-stu-id="fd288-118">groove</span></span>|<span data-ttu-id="fd288-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd288-119">Boolean</span></span>|<span data-ttu-id="fd288-120">Der Wert für die If MS Office OneDrive for Business - Groove ausgeschlossen werden soll, oder nicht.</span><span class="sxs-lookup"><span data-stu-id="fd288-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="fd288-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="fd288-121">infoPath</span></span>|<span data-ttu-id="fd288-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd288-122">Boolean</span></span>|<span data-ttu-id="fd288-123">Der Wert für die If MS Office InfoPath davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="fd288-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="fd288-124">Lync</span><span class="sxs-lookup"><span data-stu-id="fd288-124">lync</span></span>|<span data-ttu-id="fd288-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd288-125">Boolean</span></span>|<span data-ttu-id="fd288-126">Der Wert für die If MS Office Skype for Business – Lync ausgeschlossen werden soll, oder nicht.</span><span class="sxs-lookup"><span data-stu-id="fd288-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="fd288-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="fd288-127">oneDrive</span></span>|<span data-ttu-id="fd288-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd288-128">Boolean</span></span>|<span data-ttu-id="fd288-129">Der Wert für die If MS Office OneDrive davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="fd288-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="fd288-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="fd288-130">oneNote</span></span>|<span data-ttu-id="fd288-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd288-131">Boolean</span></span>|<span data-ttu-id="fd288-132">Der Wert für die If MS Office OneNote davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="fd288-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="fd288-133">Outlook</span><span class="sxs-lookup"><span data-stu-id="fd288-133">outlook</span></span>|<span data-ttu-id="fd288-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd288-134">Boolean</span></span>|<span data-ttu-id="fd288-135">Der Wert für die If MS Office Outlook oder nicht ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="fd288-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="fd288-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="fd288-136">powerPoint</span></span>|<span data-ttu-id="fd288-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd288-137">Boolean</span></span>|<span data-ttu-id="fd288-138">Der Wert für die If MS Office PowerPoint davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="fd288-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="fd288-139">publisher</span><span class="sxs-lookup"><span data-stu-id="fd288-139">publisher</span></span>|<span data-ttu-id="fd288-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd288-140">Boolean</span></span>|<span data-ttu-id="fd288-141">Der Wert für die If MS Office Publisher davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="fd288-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="fd288-142">SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="fd288-142">sharePointDesigner</span></span>|<span data-ttu-id="fd288-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd288-143">Boolean</span></span>|<span data-ttu-id="fd288-144">Der Wert für die If MS Office SharePoint Designer davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="fd288-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="fd288-145">Visio</span><span class="sxs-lookup"><span data-stu-id="fd288-145">visio</span></span>|<span data-ttu-id="fd288-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd288-146">Boolean</span></span>|<span data-ttu-id="fd288-147">Der Wert für die If MS Office Visio davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="fd288-147">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="fd288-148">Word</span><span class="sxs-lookup"><span data-stu-id="fd288-148">word</span></span>|<span data-ttu-id="fd288-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd288-149">Boolean</span></span>|<span data-ttu-id="fd288-150">Der Wert für die If MS Office Word davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="fd288-150">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd288-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fd288-151">Relationships</span></span>
<span data-ttu-id="fd288-152">Keine</span><span class="sxs-lookup"><span data-stu-id="fd288-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd288-153">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fd288-153">JSON Representation</span></span>
<span data-ttu-id="fd288-154">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fd288-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludedApps",
  "access": true,
  "excel": true,
  "groove": true,
  "infoPath": true,
  "lync": true,
  "oneDrive": true,
  "oneNote": true,
  "outlook": true,
  "powerPoint": true,
  "publisher": true,
  "sharePointDesigner": true,
  "visio": true,
  "word": true
}
```




