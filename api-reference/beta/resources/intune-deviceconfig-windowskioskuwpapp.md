---
title: windowsKioskUWPApp-Ressourcentyp
description: Die Basisklasse für eine Art von apps
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a247c3f02dc64657ec9cd297d8fff5d8591549cd
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572537"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="115bd-103">windowsKioskUWPApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="115bd-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="115bd-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="115bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="115bd-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="115bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="115bd-106">Die Basisklasse für eine Art von apps</span><span class="sxs-lookup"><span data-stu-id="115bd-106">The base class for a type of apps</span></span>


<span data-ttu-id="115bd-107">Erbt von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="115bd-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="115bd-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="115bd-108">Properties</span></span>
|<span data-ttu-id="115bd-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="115bd-109">Property</span></span>|<span data-ttu-id="115bd-110">Typ</span><span class="sxs-lookup"><span data-stu-id="115bd-110">Type</span></span>|<span data-ttu-id="115bd-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="115bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="115bd-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="115bd-112">startLayoutTileSize</span></span>|[<span data-ttu-id="115bd-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="115bd-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="115bd-114">Die Größe der APP-Kachel für das von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)geerbte Start Layout.</span><span class="sxs-lookup"><span data-stu-id="115bd-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="115bd-115">Mögliche Werte: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="115bd-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="115bd-116">name</span><span class="sxs-lookup"><span data-stu-id="115bd-116">name</span></span>|<span data-ttu-id="115bd-117">String</span><span class="sxs-lookup"><span data-stu-id="115bd-117">String</span></span>|<span data-ttu-id="115bd-118">Stellt den Anzeigenamen einer von [zum](../resources/intune-deviceconfig-windowskioskappbase.md) geerbten App dar.</span><span class="sxs-lookup"><span data-stu-id="115bd-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="115bd-119">appType</span><span class="sxs-lookup"><span data-stu-id="115bd-119">appType</span></span>|[<span data-ttu-id="115bd-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="115bd-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="115bd-121">Der von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)geerbte App-Typ.</span><span class="sxs-lookup"><span data-stu-id="115bd-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="115bd-122">Mögliche Werte sind: `unknown`, `store`, `desktop` und `aumId`.</span><span class="sxs-lookup"><span data-stu-id="115bd-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="115bd-123">Autostart</span><span class="sxs-lookup"><span data-stu-id="115bd-123">autoLaunch</span></span>|<span data-ttu-id="115bd-124">Boolesch</span><span class="sxs-lookup"><span data-stu-id="115bd-124">Boolean</span></span>|<span data-ttu-id="115bd-125">Automatisches Starten der APP im Multi-App Kiosk-Modus, geerbt von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="115bd-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="115bd-126">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="115bd-126">appUserModelId</span></span>|<span data-ttu-id="115bd-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="115bd-127">String</span></span>|<span data-ttu-id="115bd-128">Dies ist die einzige Anwendungsbenutzer Modell-ID (AUMID), die im Kiosk-Modus verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="115bd-128">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="115bd-129">appId</span><span class="sxs-lookup"><span data-stu-id="115bd-129">appId</span></span>|<span data-ttu-id="115bd-130">String</span><span class="sxs-lookup"><span data-stu-id="115bd-130">String</span></span>|<span data-ttu-id="115bd-131">Dies verweist auf eine InTune-APP, die auf die gleichen Zuordnungen wie die Kiosk Konfiguration ausgerichtet sein wird.</span><span class="sxs-lookup"><span data-stu-id="115bd-131">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="115bd-132">containedAppId</span><span class="sxs-lookup"><span data-stu-id="115bd-132">containedAppId</span></span>|<span data-ttu-id="115bd-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="115bd-133">String</span></span>|<span data-ttu-id="115bd-134">Dieser Verweis auf eine enthaltene App aus einer InTune-App</span><span class="sxs-lookup"><span data-stu-id="115bd-134">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="115bd-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="115bd-135">Relationships</span></span>
<span data-ttu-id="115bd-136">Keine</span><span class="sxs-lookup"><span data-stu-id="115bd-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="115bd-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="115bd-137">JSON Representation</span></span>
<span data-ttu-id="115bd-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="115bd-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskUWPApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```




