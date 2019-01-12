---
title: windowsInformationProtectionDesktopApp-Ressourcentyp
description: Desktop-App für Windows-Informationsschutz
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ba45dd4f3bb450cfc9822fb68f1b4511f69da2fa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977388"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="c43ba-103">windowsInformationProtectionDesktopApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c43ba-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="c43ba-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c43ba-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c43ba-105">Desktop-App für Windows-Informationsschutz</span><span class="sxs-lookup"><span data-stu-id="c43ba-105">Desktop App for Windows information protection</span></span>

<span data-ttu-id="c43ba-106">Erbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c43ba-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c43ba-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c43ba-107">Properties</span></span>
|<span data-ttu-id="c43ba-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c43ba-108">Property</span></span>|<span data-ttu-id="c43ba-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c43ba-109">Type</span></span>|<span data-ttu-id="c43ba-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c43ba-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c43ba-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c43ba-111">displayName</span></span>|<span data-ttu-id="c43ba-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c43ba-112">String</span></span>|<span data-ttu-id="c43ba-113">Anzeigename der App.</span><span class="sxs-lookup"><span data-stu-id="c43ba-113">App display name.</span></span> <span data-ttu-id="c43ba-114">Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c43ba-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c43ba-115">description</span><span class="sxs-lookup"><span data-stu-id="c43ba-115">description</span></span>|<span data-ttu-id="c43ba-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c43ba-116">String</span></span>|<span data-ttu-id="c43ba-117">Die Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="c43ba-117">The app's description.</span></span> <span data-ttu-id="c43ba-118">Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c43ba-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c43ba-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="c43ba-119">publisherName</span></span>|<span data-ttu-id="c43ba-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c43ba-120">String</span></span>|<span data-ttu-id="c43ba-121">Der Name des Herausgebers, geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c43ba-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c43ba-122">productName</span><span class="sxs-lookup"><span data-stu-id="c43ba-122">productName</span></span>|<span data-ttu-id="c43ba-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c43ba-123">String</span></span>|<span data-ttu-id="c43ba-124">Der Produktname.</span><span class="sxs-lookup"><span data-stu-id="c43ba-124">The product name.</span></span> <span data-ttu-id="c43ba-125">Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c43ba-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c43ba-126">denied</span><span class="sxs-lookup"><span data-stu-id="c43ba-126">denied</span></span>|<span data-ttu-id="c43ba-127">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c43ba-127">Boolean</span></span>|<span data-ttu-id="c43ba-128">Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert.</span><span class="sxs-lookup"><span data-stu-id="c43ba-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="c43ba-129">Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c43ba-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c43ba-130">binaryName</span><span class="sxs-lookup"><span data-stu-id="c43ba-130">binaryName</span></span>|<span data-ttu-id="c43ba-131">String</span><span class="sxs-lookup"><span data-stu-id="c43ba-131">String</span></span>|<span data-ttu-id="c43ba-132">Der binäre Name</span><span class="sxs-lookup"><span data-stu-id="c43ba-132">The binary name.</span></span>|
|<span data-ttu-id="c43ba-133">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="c43ba-133">binaryVersionLow</span></span>|<span data-ttu-id="c43ba-134">String</span><span class="sxs-lookup"><span data-stu-id="c43ba-134">String</span></span>|<span data-ttu-id="c43ba-135">Die niedrigere Binärversion.</span><span class="sxs-lookup"><span data-stu-id="c43ba-135">The lower binary version.</span></span>|
|<span data-ttu-id="c43ba-136">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="c43ba-136">binaryVersionHigh</span></span>|<span data-ttu-id="c43ba-137">String</span><span class="sxs-lookup"><span data-stu-id="c43ba-137">String</span></span>|<span data-ttu-id="c43ba-138">Die größte Binärversion.</span><span class="sxs-lookup"><span data-stu-id="c43ba-138">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c43ba-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c43ba-139">Relationships</span></span>
<span data-ttu-id="c43ba-140">Keine</span><span class="sxs-lookup"><span data-stu-id="c43ba-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c43ba-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c43ba-141">JSON Representation</span></span>
<span data-ttu-id="c43ba-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c43ba-142">Here is a JSON representation of the resource.</span></span>
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



