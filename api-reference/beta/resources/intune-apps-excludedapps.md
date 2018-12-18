---
title: Ressourcentyp excludedApps
description: Enthält Eigenschaften für die ausgeschlossenen Office365 Apps.
author: tfitzmac
ms.openlocfilehash: b8c9eff985783c953ff099dbf4d5ba00826652c4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344625"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="c1648-103">Ressourcentyp excludedApps</span><span class="sxs-lookup"><span data-stu-id="c1648-103">excludedApps resource type</span></span>

> <span data-ttu-id="c1648-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c1648-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1648-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c1648-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1648-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c1648-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1648-107">Enthält Eigenschaften für die ausgeschlossenen Office365 Apps.</span><span class="sxs-lookup"><span data-stu-id="c1648-107">Contains properties for Excluded Office365 Apps.</span></span>
## <a name="properties"></a><span data-ttu-id="c1648-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c1648-108">Properties</span></span>
|<span data-ttu-id="c1648-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c1648-109">Property</span></span>|<span data-ttu-id="c1648-110">Typ</span><span class="sxs-lookup"><span data-stu-id="c1648-110">Type</span></span>|<span data-ttu-id="c1648-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1648-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1648-112">access</span><span class="sxs-lookup"><span data-stu-id="c1648-112">access</span></span>|<span data-ttu-id="c1648-113">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c1648-113">Boolean</span></span>|<span data-ttu-id="c1648-114">Der Wert für die If MS Office Access davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1648-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="c1648-115">Excel-</span><span class="sxs-lookup"><span data-stu-id="c1648-115">excel</span></span>|<span data-ttu-id="c1648-116">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c1648-116">Boolean</span></span>|<span data-ttu-id="c1648-117">Der Wert für die If MS Office Excel davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1648-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="c1648-118">Groove</span><span class="sxs-lookup"><span data-stu-id="c1648-118">groove</span></span>|<span data-ttu-id="c1648-119">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c1648-119">Boolean</span></span>|<span data-ttu-id="c1648-120">Der Wert für die If MS Office OneDrive for Business - Groove ausgeschlossen werden soll, oder nicht.</span><span class="sxs-lookup"><span data-stu-id="c1648-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="c1648-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="c1648-121">infoPath</span></span>|<span data-ttu-id="c1648-122">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c1648-122">Boolean</span></span>|<span data-ttu-id="c1648-123">Der Wert für die If MS Office InfoPath davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1648-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="c1648-124">Lync</span><span class="sxs-lookup"><span data-stu-id="c1648-124">lync</span></span>|<span data-ttu-id="c1648-125">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c1648-125">Boolean</span></span>|<span data-ttu-id="c1648-126">Der Wert für die If MS Office Skype for Business – Lync ausgeschlossen werden soll, oder nicht.</span><span class="sxs-lookup"><span data-stu-id="c1648-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="c1648-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="c1648-127">oneDrive</span></span>|<span data-ttu-id="c1648-128">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c1648-128">Boolean</span></span>|<span data-ttu-id="c1648-129">Der Wert für die If MS Office OneDrive davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1648-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="c1648-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="c1648-130">oneNote</span></span>|<span data-ttu-id="c1648-131">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c1648-131">Boolean</span></span>|<span data-ttu-id="c1648-132">Der Wert für die If MS Office OneNote davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1648-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="c1648-133">Outlook</span><span class="sxs-lookup"><span data-stu-id="c1648-133">outlook</span></span>|<span data-ttu-id="c1648-134">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c1648-134">Boolean</span></span>|<span data-ttu-id="c1648-135">Der Wert für die If MS Office Outlook oder nicht ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1648-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="c1648-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="c1648-136">powerPoint</span></span>|<span data-ttu-id="c1648-137">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c1648-137">Boolean</span></span>|<span data-ttu-id="c1648-138">Der Wert für die If MS Office PowerPoint davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1648-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="c1648-139">publisher</span><span class="sxs-lookup"><span data-stu-id="c1648-139">publisher</span></span>|<span data-ttu-id="c1648-140">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c1648-140">Boolean</span></span>|<span data-ttu-id="c1648-141">Der Wert für die If MS Office Publisher davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1648-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="c1648-142">SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="c1648-142">sharePointDesigner</span></span>|<span data-ttu-id="c1648-143">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c1648-143">Boolean</span></span>|<span data-ttu-id="c1648-144">Der Wert für die If MS Office SharePoint Designer davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1648-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="c1648-145">Visio</span><span class="sxs-lookup"><span data-stu-id="c1648-145">visio</span></span>|<span data-ttu-id="c1648-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c1648-146">Boolean</span></span>|<span data-ttu-id="c1648-147">Der Wert für die If MS Office Visio davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1648-147">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="c1648-148">Word</span><span class="sxs-lookup"><span data-stu-id="c1648-148">word</span></span>|<span data-ttu-id="c1648-149">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c1648-149">Boolean</span></span>|<span data-ttu-id="c1648-150">Der Wert für die If MS Office Word davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1648-150">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1648-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c1648-151">Relationships</span></span>
<span data-ttu-id="c1648-152">Keine</span><span class="sxs-lookup"><span data-stu-id="c1648-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c1648-153">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c1648-153">JSON Representation</span></span>
<span data-ttu-id="c1648-154">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c1648-154">Here is a JSON representation of the resource.</span></span>
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





