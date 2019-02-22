---
title: windowsKioskDesktopApp-Ressourcentyp
description: Die Basisklasse für eine Art von apps
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0487fa24ecd2d27817349b68063cf606a2401944
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170476"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="26e5b-103">windowsKioskDesktopApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="26e5b-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="26e5b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="26e5b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26e5b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="26e5b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26e5b-106">Die Basisklasse für eine Art von apps</span><span class="sxs-lookup"><span data-stu-id="26e5b-106">The base class for a type of apps</span></span>


<span data-ttu-id="26e5b-107">Erbt von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="26e5b-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="26e5b-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="26e5b-108">Properties</span></span>
|<span data-ttu-id="26e5b-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="26e5b-109">Property</span></span>|<span data-ttu-id="26e5b-110">Typ</span><span class="sxs-lookup"><span data-stu-id="26e5b-110">Type</span></span>|<span data-ttu-id="26e5b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26e5b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26e5b-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="26e5b-112">startLayoutTileSize</span></span>|[<span data-ttu-id="26e5b-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="26e5b-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="26e5b-114">Die Größe der APP-Kachel für das von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)geerbte Start Layout.</span><span class="sxs-lookup"><span data-stu-id="26e5b-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="26e5b-115">Mögliche Werte: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="26e5b-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="26e5b-116">name</span><span class="sxs-lookup"><span data-stu-id="26e5b-116">name</span></span>|<span data-ttu-id="26e5b-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26e5b-117">String</span></span>|<span data-ttu-id="26e5b-118">Stellt den Anzeigenamen einer von [zum](../resources/intune-deviceconfig-windowskioskappbase.md) geerbten App dar.</span><span class="sxs-lookup"><span data-stu-id="26e5b-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="26e5b-119">appType</span><span class="sxs-lookup"><span data-stu-id="26e5b-119">appType</span></span>|[<span data-ttu-id="26e5b-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="26e5b-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="26e5b-121">Der von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)geerbte App-Typ.</span><span class="sxs-lookup"><span data-stu-id="26e5b-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="26e5b-122">Mögliche Werte: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="26e5b-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="26e5b-123">Pfad</span><span class="sxs-lookup"><span data-stu-id="26e5b-123">path</span></span>|<span data-ttu-id="26e5b-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26e5b-124">String</span></span>|<span data-ttu-id="26e5b-125">Definieren des Pfads einer Desktop-App</span><span class="sxs-lookup"><span data-stu-id="26e5b-125">Define the path of a desktop app</span></span>|
|<span data-ttu-id="26e5b-126">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="26e5b-126">desktopApplicationId</span></span>|<span data-ttu-id="26e5b-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26e5b-127">String</span></span>|<span data-ttu-id="26e5b-128">Definieren der DesktopApplicationID der APP</span><span class="sxs-lookup"><span data-stu-id="26e5b-128">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="26e5b-129">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="26e5b-129">desktopApplicationLinkPath</span></span>|<span data-ttu-id="26e5b-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26e5b-130">String</span></span>|<span data-ttu-id="26e5b-131">Definieren der DesktopApplicationLinkPath der APP</span><span class="sxs-lookup"><span data-stu-id="26e5b-131">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="26e5b-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="26e5b-132">Relationships</span></span>
<span data-ttu-id="26e5b-133">Keine</span><span class="sxs-lookup"><span data-stu-id="26e5b-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26e5b-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="26e5b-134">JSON Representation</span></span>
<span data-ttu-id="26e5b-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="26e5b-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskDesktopApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```




