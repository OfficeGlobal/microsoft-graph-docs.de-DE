---
title: Ressourcentyp excludedApps
description: Enthält Eigenschaften für die ausgeschlossenen Office365 Apps.
ms.openlocfilehash: 05c1ed7f4789e1a27ddacf92dbd773b2f5a21847
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060566"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="c0cec-103">Ressourcentyp excludedApps</span><span class="sxs-lookup"><span data-stu-id="c0cec-103">excludedApps resource type</span></span>

> <span data-ttu-id="c0cec-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c0cec-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0cec-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0cec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0cec-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c0cec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0cec-107">Enthält Eigenschaften für die ausgeschlossenen Office365 Apps.</span><span class="sxs-lookup"><span data-stu-id="c0cec-107">Contains properties for Excluded Office365 Apps.</span></span>
## <a name="properties"></a><span data-ttu-id="c0cec-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c0cec-108">Properties</span></span>
|<span data-ttu-id="c0cec-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c0cec-109">Property</span></span>|<span data-ttu-id="c0cec-110">Typ</span><span class="sxs-lookup"><span data-stu-id="c0cec-110">Type</span></span>|<span data-ttu-id="c0cec-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0cec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0cec-112">Zugriff</span><span class="sxs-lookup"><span data-stu-id="c0cec-112">access</span></span>|<span data-ttu-id="c0cec-113">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c0cec-113">Boolean</span></span>|<span data-ttu-id="c0cec-114">Der Wert für die If MS Office Access davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c0cec-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="c0cec-115">Excel-</span><span class="sxs-lookup"><span data-stu-id="c0cec-115">excel</span></span>|<span data-ttu-id="c0cec-116">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c0cec-116">Boolean</span></span>|<span data-ttu-id="c0cec-117">Der Wert für die If MS Office Excel davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c0cec-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="c0cec-118">Groove</span><span class="sxs-lookup"><span data-stu-id="c0cec-118">groove</span></span>|<span data-ttu-id="c0cec-119">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c0cec-119">Boolean</span></span>|<span data-ttu-id="c0cec-120">Der Wert für die If MS Office OneDrive for Business - Groove ausgeschlossen werden soll, oder nicht.</span><span class="sxs-lookup"><span data-stu-id="c0cec-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="c0cec-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="c0cec-121">infoPath</span></span>|<span data-ttu-id="c0cec-122">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c0cec-122">Boolean</span></span>|<span data-ttu-id="c0cec-123">Der Wert für die If MS Office InfoPath davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c0cec-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="c0cec-124">Lync</span><span class="sxs-lookup"><span data-stu-id="c0cec-124">lync</span></span>|<span data-ttu-id="c0cec-125">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c0cec-125">Boolean</span></span>|<span data-ttu-id="c0cec-126">Der Wert für die If MS Office Skype for Business – Lync ausgeschlossen werden soll, oder nicht.</span><span class="sxs-lookup"><span data-stu-id="c0cec-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="c0cec-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="c0cec-127">oneDrive</span></span>|<span data-ttu-id="c0cec-128">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c0cec-128">Boolean</span></span>|<span data-ttu-id="c0cec-129">Der Wert für die If MS Office OneDrive davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c0cec-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="c0cec-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="c0cec-130">oneNote</span></span>|<span data-ttu-id="c0cec-131">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c0cec-131">Boolean</span></span>|<span data-ttu-id="c0cec-132">Der Wert für die If MS Office OneNote davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c0cec-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="c0cec-133">Outlook</span><span class="sxs-lookup"><span data-stu-id="c0cec-133">outlook</span></span>|<span data-ttu-id="c0cec-134">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c0cec-134">Boolean</span></span>|<span data-ttu-id="c0cec-135">Der Wert für die If MS Office Outlook oder nicht ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c0cec-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="c0cec-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="c0cec-136">powerPoint</span></span>|<span data-ttu-id="c0cec-137">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c0cec-137">Boolean</span></span>|<span data-ttu-id="c0cec-138">Der Wert für die If MS Office PowerPoint davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c0cec-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="c0cec-139">publisher</span><span class="sxs-lookup"><span data-stu-id="c0cec-139">publisher</span></span>|<span data-ttu-id="c0cec-140">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c0cec-140">Boolean</span></span>|<span data-ttu-id="c0cec-141">Der Wert für die If MS Office Publisher davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c0cec-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="c0cec-142">SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="c0cec-142">sharePointDesigner</span></span>|<span data-ttu-id="c0cec-143">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c0cec-143">Boolean</span></span>|<span data-ttu-id="c0cec-144">Der Wert für die If MS Office SharePoint Designer davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c0cec-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="c0cec-145">Visio</span><span class="sxs-lookup"><span data-stu-id="c0cec-145">visio</span></span>|<span data-ttu-id="c0cec-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c0cec-146">Boolean</span></span>|<span data-ttu-id="c0cec-147">Der Wert für die If MS Office Visio davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c0cec-147">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="c0cec-148">Word</span><span class="sxs-lookup"><span data-stu-id="c0cec-148">word</span></span>|<span data-ttu-id="c0cec-149">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c0cec-149">Boolean</span></span>|<span data-ttu-id="c0cec-150">Der Wert für die If MS Office Word davon ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="c0cec-150">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0cec-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c0cec-151">Relationships</span></span>
<span data-ttu-id="c0cec-152">Keine</span><span class="sxs-lookup"><span data-stu-id="c0cec-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c0cec-153">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c0cec-153">JSON Representation</span></span>
<span data-ttu-id="c0cec-154">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c0cec-154">Here is a JSON representation of the resource.</span></span>
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





