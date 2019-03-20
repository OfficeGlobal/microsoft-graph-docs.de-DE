---
title: Zum-Ressourcentyp
description: Die Basisklasse für eine Art von apps
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b86921fcdaa11b37b985184dfbc645c2a193bfdb
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572306"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="f351d-103">Zum-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f351d-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="f351d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f351d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f351d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f351d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f351d-106">Die Basisklasse für eine Art von apps</span><span class="sxs-lookup"><span data-stu-id="f351d-106">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="f351d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f351d-107">Properties</span></span>
|<span data-ttu-id="f351d-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f351d-108">Property</span></span>|<span data-ttu-id="f351d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f351d-109">Type</span></span>|<span data-ttu-id="f351d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f351d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f351d-111">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="f351d-111">startLayoutTileSize</span></span>|[<span data-ttu-id="f351d-112">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="f351d-112">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="f351d-113">Die Größe der APP-Kachel für das Start Layout.</span><span class="sxs-lookup"><span data-stu-id="f351d-113">The app tile size for the start layout.</span></span> <span data-ttu-id="f351d-114">Mögliche Werte: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="f351d-114">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="f351d-115">name</span><span class="sxs-lookup"><span data-stu-id="f351d-115">name</span></span>|<span data-ttu-id="f351d-116">String</span><span class="sxs-lookup"><span data-stu-id="f351d-116">String</span></span>|<span data-ttu-id="f351d-117">Stellt den Anzeigenamen einer APP dar.</span><span class="sxs-lookup"><span data-stu-id="f351d-117">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="f351d-118">appType</span><span class="sxs-lookup"><span data-stu-id="f351d-118">appType</span></span>|[<span data-ttu-id="f351d-119">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="f351d-119">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="f351d-120">Der APP-Typ.</span><span class="sxs-lookup"><span data-stu-id="f351d-120">The app type.</span></span> <span data-ttu-id="f351d-121">Mögliche Werte sind: `unknown`, `store`, `desktop` und `aumId`.</span><span class="sxs-lookup"><span data-stu-id="f351d-121">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="f351d-122">Autostart</span><span class="sxs-lookup"><span data-stu-id="f351d-122">autoLaunch</span></span>|<span data-ttu-id="f351d-123">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f351d-123">Boolean</span></span>|<span data-ttu-id="f351d-124">Automatisches Starten der APP im Multi-App Kiosk-Modus</span><span class="sxs-lookup"><span data-stu-id="f351d-124">Allow the app to be auto-launched in multi-app kiosk mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="f351d-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f351d-125">Relationships</span></span>
<span data-ttu-id="f351d-126">Keine</span><span class="sxs-lookup"><span data-stu-id="f351d-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f351d-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f351d-127">JSON Representation</span></span>
<span data-ttu-id="f351d-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f351d-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAppBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAppBase",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true
}
```




