---
title: excludedApps-Ressourcentyp
description: Enthält Eigenschaften für ausgeschlossene Office365-apps.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8dee0d5328f1f69c95159116bf913bc2abb959d7
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571690"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="2146d-103">excludedApps-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2146d-103">excludedApps resource type</span></span>

> <span data-ttu-id="2146d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2146d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2146d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2146d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2146d-106">Enthält Eigenschaften für ausgeschlossene Office365-apps.</span><span class="sxs-lookup"><span data-stu-id="2146d-106">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="2146d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2146d-107">Properties</span></span>
|<span data-ttu-id="2146d-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2146d-108">Property</span></span>|<span data-ttu-id="2146d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="2146d-109">Type</span></span>|<span data-ttu-id="2146d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2146d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2146d-111">Access</span><span class="sxs-lookup"><span data-stu-id="2146d-111">access</span></span>|<span data-ttu-id="2146d-112">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2146d-112">Boolean</span></span>|<span data-ttu-id="2146d-113">Der Wert für, wenn MS Office Access ausgeschlossen werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="2146d-113">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="2146d-114">Excel</span><span class="sxs-lookup"><span data-stu-id="2146d-114">excel</span></span>|<span data-ttu-id="2146d-115">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2146d-115">Boolean</span></span>|<span data-ttu-id="2146d-116">Der Wert für, wenn MS Office Excel ausgeschlossen werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="2146d-116">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="2146d-117">Groove</span><span class="sxs-lookup"><span data-stu-id="2146d-117">groove</span></span>|<span data-ttu-id="2146d-118">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2146d-118">Boolean</span></span>|<span data-ttu-id="2146d-119">Der Wert für IF MS Office OneDrive for Business-Groove sollte ausgeschlossen werden oder nicht.</span><span class="sxs-lookup"><span data-stu-id="2146d-119">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="2146d-120">infoPath</span><span class="sxs-lookup"><span data-stu-id="2146d-120">infoPath</span></span>|<span data-ttu-id="2146d-121">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2146d-121">Boolean</span></span>|<span data-ttu-id="2146d-122">Der Wert für, wenn MS Office InfoPath ausgeschlossen werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="2146d-122">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="2146d-123">lync</span><span class="sxs-lookup"><span data-stu-id="2146d-123">lync</span></span>|<span data-ttu-id="2146d-124">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2146d-124">Boolean</span></span>|<span data-ttu-id="2146d-125">Der Wert für, wenn MS Office Skype for Business-lync ausgeschlossen werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="2146d-125">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="2146d-126">oneDrive</span><span class="sxs-lookup"><span data-stu-id="2146d-126">oneDrive</span></span>|<span data-ttu-id="2146d-127">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2146d-127">Boolean</span></span>|<span data-ttu-id="2146d-128">Der Wert für, wenn MS Office OneDrive ausgeschlossen werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="2146d-128">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="2146d-129">oneNote</span><span class="sxs-lookup"><span data-stu-id="2146d-129">oneNote</span></span>|<span data-ttu-id="2146d-130">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2146d-130">Boolean</span></span>|<span data-ttu-id="2146d-131">Der Wert für, wenn MS Office OneNote ausgeschlossen werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="2146d-131">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="2146d-132">outlook</span><span class="sxs-lookup"><span data-stu-id="2146d-132">outlook</span></span>|<span data-ttu-id="2146d-133">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2146d-133">Boolean</span></span>|<span data-ttu-id="2146d-134">Der Wert für, wenn MS Office Outlook ausgeschlossen werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="2146d-134">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="2146d-135">Kulissen</span><span class="sxs-lookup"><span data-stu-id="2146d-135">powerPoint</span></span>|<span data-ttu-id="2146d-136">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2146d-136">Boolean</span></span>|<span data-ttu-id="2146d-137">Der Wert für IF MS Office PowerPoint sollte ausgeschlossen werden oder nicht.</span><span class="sxs-lookup"><span data-stu-id="2146d-137">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="2146d-138">publisher</span><span class="sxs-lookup"><span data-stu-id="2146d-138">publisher</span></span>|<span data-ttu-id="2146d-139">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2146d-139">Boolean</span></span>|<span data-ttu-id="2146d-140">Der Wert für, wenn MS Office Publisher ausgeschlossen werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="2146d-140">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="2146d-141">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="2146d-141">sharePointDesigner</span></span>|<span data-ttu-id="2146d-142">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2146d-142">Boolean</span></span>|<span data-ttu-id="2146d-143">Der Wert für, wenn MS Office SharePointDesigner ausgeschlossen werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="2146d-143">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="2146d-144">Teams</span><span class="sxs-lookup"><span data-stu-id="2146d-144">teams</span></span>|<span data-ttu-id="2146d-145">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2146d-145">Boolean</span></span>|<span data-ttu-id="2146d-146">Der Wert für IF-MS Office Teams sollte ausgeschlossen werden oder nicht.</span><span class="sxs-lookup"><span data-stu-id="2146d-146">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="2146d-147">Visio</span><span class="sxs-lookup"><span data-stu-id="2146d-147">visio</span></span>|<span data-ttu-id="2146d-148">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2146d-148">Boolean</span></span>|<span data-ttu-id="2146d-149">Der Wert für, wenn MS Office Visio ausgeschlossen werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="2146d-149">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="2146d-150">Wort</span><span class="sxs-lookup"><span data-stu-id="2146d-150">word</span></span>|<span data-ttu-id="2146d-151">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2146d-151">Boolean</span></span>|<span data-ttu-id="2146d-152">Der Wert für, wenn MS Office Word ausgeschlossen werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="2146d-152">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2146d-153">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2146d-153">Relationships</span></span>
<span data-ttu-id="2146d-154">Keine</span><span class="sxs-lookup"><span data-stu-id="2146d-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2146d-155">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2146d-155">JSON Representation</span></span>
<span data-ttu-id="2146d-156">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2146d-156">Here is a JSON representation of the resource.</span></span>
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
  "teams": true,
  "visio": true,
  "word": true
}
```




