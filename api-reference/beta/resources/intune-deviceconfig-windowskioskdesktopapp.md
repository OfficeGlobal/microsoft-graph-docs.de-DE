---
title: windowsKioskDesktopApp-Ressourcentyp
description: Die Basisklasse für eine Art von apps
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4cccd1b5e7ec7ca16aeb76b87fc31d90e92e7dcd
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30572082"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="6ec84-103">windowsKioskDesktopApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6ec84-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="6ec84-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6ec84-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ec84-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6ec84-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ec84-106">Die Basisklasse für eine Art von apps</span><span class="sxs-lookup"><span data-stu-id="6ec84-106">The base class for a type of apps</span></span>


<span data-ttu-id="6ec84-107">Erbt von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="6ec84-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6ec84-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6ec84-108">Properties</span></span>
|<span data-ttu-id="6ec84-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6ec84-109">Property</span></span>|<span data-ttu-id="6ec84-110">Typ</span><span class="sxs-lookup"><span data-stu-id="6ec84-110">Type</span></span>|<span data-ttu-id="6ec84-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ec84-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ec84-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="6ec84-112">startLayoutTileSize</span></span>|[<span data-ttu-id="6ec84-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="6ec84-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="6ec84-114">Die Größe der APP-Kachel für das von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)geerbte Start Layout.</span><span class="sxs-lookup"><span data-stu-id="6ec84-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="6ec84-115">Mögliche Werte: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="6ec84-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="6ec84-116">name</span><span class="sxs-lookup"><span data-stu-id="6ec84-116">name</span></span>|<span data-ttu-id="6ec84-117">String</span><span class="sxs-lookup"><span data-stu-id="6ec84-117">String</span></span>|<span data-ttu-id="6ec84-118">Stellt den Anzeigenamen einer von [zum](../resources/intune-deviceconfig-windowskioskappbase.md) geerbten App dar.</span><span class="sxs-lookup"><span data-stu-id="6ec84-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="6ec84-119">appType</span><span class="sxs-lookup"><span data-stu-id="6ec84-119">appType</span></span>|[<span data-ttu-id="6ec84-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="6ec84-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="6ec84-121">Der von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)geerbte App-Typ.</span><span class="sxs-lookup"><span data-stu-id="6ec84-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="6ec84-122">Mögliche Werte sind: `unknown`, `store`, `desktop` und `aumId`.</span><span class="sxs-lookup"><span data-stu-id="6ec84-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="6ec84-123">Autostart</span><span class="sxs-lookup"><span data-stu-id="6ec84-123">autoLaunch</span></span>|<span data-ttu-id="6ec84-124">Boolesch</span><span class="sxs-lookup"><span data-stu-id="6ec84-124">Boolean</span></span>|<span data-ttu-id="6ec84-125">Automatisches Starten der APP im Multi-App Kiosk-Modus, geerbt von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="6ec84-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="6ec84-126">Pfad</span><span class="sxs-lookup"><span data-stu-id="6ec84-126">path</span></span>|<span data-ttu-id="6ec84-127">String</span><span class="sxs-lookup"><span data-stu-id="6ec84-127">String</span></span>|<span data-ttu-id="6ec84-128">Definieren des Pfads einer Desktop-App</span><span class="sxs-lookup"><span data-stu-id="6ec84-128">Define the path of a desktop app</span></span>|
|<span data-ttu-id="6ec84-129">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="6ec84-129">desktopApplicationId</span></span>|<span data-ttu-id="6ec84-130">String</span><span class="sxs-lookup"><span data-stu-id="6ec84-130">String</span></span>|<span data-ttu-id="6ec84-131">Definieren der DesktopApplicationID der APP</span><span class="sxs-lookup"><span data-stu-id="6ec84-131">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="6ec84-132">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="6ec84-132">desktopApplicationLinkPath</span></span>|<span data-ttu-id="6ec84-133">String</span><span class="sxs-lookup"><span data-stu-id="6ec84-133">String</span></span>|<span data-ttu-id="6ec84-134">Definieren der DesktopApplicationLinkPath der APP</span><span class="sxs-lookup"><span data-stu-id="6ec84-134">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ec84-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6ec84-135">Relationships</span></span>
<span data-ttu-id="6ec84-136">Keine</span><span class="sxs-lookup"><span data-stu-id="6ec84-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ec84-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6ec84-137">JSON Representation</span></span>
<span data-ttu-id="6ec84-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6ec84-138">Here is a JSON representation of the resource.</span></span>
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
  "autoLaunch": true,
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```




