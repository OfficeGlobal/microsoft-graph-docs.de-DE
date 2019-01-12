---
title: Ressourcentyp excludedApps
description: Enthält Eigenschaften für die ausgeschlossenen Office365 Apps.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90216c639d36a989b2fad5dbdc1adbd11fe46ede
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943949"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="b8cf0-103">Ressourcentyp excludedApps</span><span class="sxs-lookup"><span data-stu-id="b8cf0-103">excludedApps resource type</span></span>

> <span data-ttu-id="b8cf0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b8cf0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8cf0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8cf0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8cf0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b8cf0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8cf0-107">Enthält Eigenschaften für die ausgeschlossenen Office365 Apps.</span><span class="sxs-lookup"><span data-stu-id="b8cf0-107">Contains properties for Excluded Office365 Apps.</span></span>
## <a name="properties"></a><span data-ttu-id="b8cf0-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b8cf0-108">Properties</span></span>
|<span data-ttu-id="b8cf0-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8cf0-109">Property</span></span>|<span data-ttu-id="b8cf0-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b8cf0-110">Type</span></span>|<span data-ttu-id="b8cf0-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8cf0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8cf0-112">access</span><span class="sxs-lookup"><span data-stu-id="b8cf0-112">access</span></span>|<span data-ttu-id="b8cf0-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8cf0-113">Boolean</span></span>|<span data-ttu-id="b8cf0-114">Der Wert für die If MS Office Access davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="b8cf0-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="b8cf0-115">Excel-</span><span class="sxs-lookup"><span data-stu-id="b8cf0-115">excel</span></span>|<span data-ttu-id="b8cf0-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8cf0-116">Boolean</span></span>|<span data-ttu-id="b8cf0-117">Der Wert für die If MS Office Excel davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="b8cf0-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="b8cf0-118">Groove</span><span class="sxs-lookup"><span data-stu-id="b8cf0-118">groove</span></span>|<span data-ttu-id="b8cf0-119">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8cf0-119">Boolean</span></span>|<span data-ttu-id="b8cf0-120">Der Wert für die If MS Office OneDrive for Business - Groove ausgeschlossen werden soll, oder nicht.</span><span class="sxs-lookup"><span data-stu-id="b8cf0-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="b8cf0-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="b8cf0-121">infoPath</span></span>|<span data-ttu-id="b8cf0-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8cf0-122">Boolean</span></span>|<span data-ttu-id="b8cf0-123">Der Wert für die If MS Office InfoPath davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="b8cf0-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="b8cf0-124">Lync</span><span class="sxs-lookup"><span data-stu-id="b8cf0-124">lync</span></span>|<span data-ttu-id="b8cf0-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8cf0-125">Boolean</span></span>|<span data-ttu-id="b8cf0-126">Der Wert für die If MS Office Skype for Business – Lync ausgeschlossen werden soll, oder nicht.</span><span class="sxs-lookup"><span data-stu-id="b8cf0-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="b8cf0-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="b8cf0-127">oneDrive</span></span>|<span data-ttu-id="b8cf0-128">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8cf0-128">Boolean</span></span>|<span data-ttu-id="b8cf0-129">Der Wert für die If MS Office OneDrive davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="b8cf0-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="b8cf0-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="b8cf0-130">oneNote</span></span>|<span data-ttu-id="b8cf0-131">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8cf0-131">Boolean</span></span>|<span data-ttu-id="b8cf0-132">Der Wert für die If MS Office OneNote davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="b8cf0-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="b8cf0-133">Outlook</span><span class="sxs-lookup"><span data-stu-id="b8cf0-133">outlook</span></span>|<span data-ttu-id="b8cf0-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8cf0-134">Boolean</span></span>|<span data-ttu-id="b8cf0-135">Der Wert für die If MS Office Outlook oder nicht ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="b8cf0-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="b8cf0-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="b8cf0-136">powerPoint</span></span>|<span data-ttu-id="b8cf0-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8cf0-137">Boolean</span></span>|<span data-ttu-id="b8cf0-138">Der Wert für die If MS Office PowerPoint davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="b8cf0-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="b8cf0-139">publisher</span><span class="sxs-lookup"><span data-stu-id="b8cf0-139">publisher</span></span>|<span data-ttu-id="b8cf0-140">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8cf0-140">Boolean</span></span>|<span data-ttu-id="b8cf0-141">Der Wert für die If MS Office Publisher davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="b8cf0-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="b8cf0-142">SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="b8cf0-142">sharePointDesigner</span></span>|<span data-ttu-id="b8cf0-143">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8cf0-143">Boolean</span></span>|<span data-ttu-id="b8cf0-144">Der Wert für die If MS Office SharePoint Designer davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="b8cf0-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="b8cf0-145">Visio</span><span class="sxs-lookup"><span data-stu-id="b8cf0-145">visio</span></span>|<span data-ttu-id="b8cf0-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8cf0-146">Boolean</span></span>|<span data-ttu-id="b8cf0-147">Der Wert für die If MS Office Visio davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="b8cf0-147">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="b8cf0-148">Word</span><span class="sxs-lookup"><span data-stu-id="b8cf0-148">word</span></span>|<span data-ttu-id="b8cf0-149">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8cf0-149">Boolean</span></span>|<span data-ttu-id="b8cf0-150">Der Wert für die If MS Office Word davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="b8cf0-150">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8cf0-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b8cf0-151">Relationships</span></span>
<span data-ttu-id="b8cf0-152">Keine</span><span class="sxs-lookup"><span data-stu-id="b8cf0-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b8cf0-153">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b8cf0-153">JSON Representation</span></span>
<span data-ttu-id="b8cf0-154">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b8cf0-154">Here is a JSON representation of the resource.</span></span>
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





