---
title: windowsInformationProtectionDesktopApp-Ressourcentyp
description: Desktop-App für Windows-Informationsschutz
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e83ad9e3e500ab5276e4643055f602e763de34fd
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259983"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="7a712-103">windowsInformationProtectionDesktopApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7a712-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="7a712-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7a712-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a712-105">Desktop-App für Windows-Informationsschutz</span><span class="sxs-lookup"><span data-stu-id="7a712-105">Desktop App for Windows information protection</span></span>


<span data-ttu-id="7a712-106">Erbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a712-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7a712-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7a712-107">Properties</span></span>
|<span data-ttu-id="7a712-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7a712-108">Property</span></span>|<span data-ttu-id="7a712-109">Typ</span><span class="sxs-lookup"><span data-stu-id="7a712-109">Type</span></span>|<span data-ttu-id="7a712-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a712-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a712-111">displayName</span><span class="sxs-lookup"><span data-stu-id="7a712-111">displayName</span></span>|<span data-ttu-id="7a712-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a712-112">String</span></span>|<span data-ttu-id="7a712-113">Anzeigename der App.</span><span class="sxs-lookup"><span data-stu-id="7a712-113">App display name.</span></span> <span data-ttu-id="7a712-114">Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a712-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="7a712-115">description</span><span class="sxs-lookup"><span data-stu-id="7a712-115">description</span></span>|<span data-ttu-id="7a712-116">String</span><span class="sxs-lookup"><span data-stu-id="7a712-116">String</span></span>|<span data-ttu-id="7a712-117">Die Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="7a712-117">The app's description.</span></span> <span data-ttu-id="7a712-118">Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a712-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="7a712-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="7a712-119">publisherName</span></span>|<span data-ttu-id="7a712-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a712-120">String</span></span>|<span data-ttu-id="7a712-121">Der Name des Herausgebers, geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a712-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="7a712-122">productName</span><span class="sxs-lookup"><span data-stu-id="7a712-122">productName</span></span>|<span data-ttu-id="7a712-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a712-123">String</span></span>|<span data-ttu-id="7a712-124">Der Produktname.</span><span class="sxs-lookup"><span data-stu-id="7a712-124">The product name.</span></span> <span data-ttu-id="7a712-125">Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a712-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="7a712-126">denied</span><span class="sxs-lookup"><span data-stu-id="7a712-126">denied</span></span>|<span data-ttu-id="7a712-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a712-127">Boolean</span></span>|<span data-ttu-id="7a712-128">Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert.</span><span class="sxs-lookup"><span data-stu-id="7a712-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="7a712-129">Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a712-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="7a712-130">binaryName</span><span class="sxs-lookup"><span data-stu-id="7a712-130">binaryName</span></span>|<span data-ttu-id="7a712-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a712-131">String</span></span>|<span data-ttu-id="7a712-132">Der binäre Name</span><span class="sxs-lookup"><span data-stu-id="7a712-132">The binary name.</span></span>|
|<span data-ttu-id="7a712-133">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="7a712-133">binaryVersionLow</span></span>|<span data-ttu-id="7a712-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a712-134">String</span></span>|<span data-ttu-id="7a712-135">Die niedrigere Binärversion.</span><span class="sxs-lookup"><span data-stu-id="7a712-135">The lower binary version.</span></span>|
|<span data-ttu-id="7a712-136">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="7a712-136">binaryVersionHigh</span></span>|<span data-ttu-id="7a712-137">String</span><span class="sxs-lookup"><span data-stu-id="7a712-137">String</span></span>|<span data-ttu-id="7a712-138">Die größte Binärversion.</span><span class="sxs-lookup"><span data-stu-id="7a712-138">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a712-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7a712-139">Relationships</span></span>
<span data-ttu-id="7a712-140">Keine</span><span class="sxs-lookup"><span data-stu-id="7a712-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a712-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7a712-141">JSON Representation</span></span>
<span data-ttu-id="7a712-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7a712-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDesktopApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true,
  "binaryName": "String",
  "binaryVersionLow": "String",
  "binaryVersionHigh": "String"
}
```



