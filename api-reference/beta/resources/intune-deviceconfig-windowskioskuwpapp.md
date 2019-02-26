---
title: windowsKioskUWPApp-Ressourcentyp
description: Die Basisklasse für eine Art von apps
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1dbaf8dfd7f2cd488de37378f934ca3f31daedd6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147327"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="b2cf6-103">windowsKioskUWPApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b2cf6-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="b2cf6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b2cf6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2cf6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b2cf6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2cf6-106">Die Basisklasse für eine Art von apps</span><span class="sxs-lookup"><span data-stu-id="b2cf6-106">The base class for a type of apps</span></span>


<span data-ttu-id="b2cf6-107">Erbt von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="b2cf6-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b2cf6-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b2cf6-108">Properties</span></span>
|<span data-ttu-id="b2cf6-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b2cf6-109">Property</span></span>|<span data-ttu-id="b2cf6-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b2cf6-110">Type</span></span>|<span data-ttu-id="b2cf6-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2cf6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2cf6-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="b2cf6-112">startLayoutTileSize</span></span>|[<span data-ttu-id="b2cf6-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="b2cf6-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="b2cf6-114">Die Größe der APP-Kachel für das von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)geerbte Start Layout.</span><span class="sxs-lookup"><span data-stu-id="b2cf6-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="b2cf6-115">Mögliche Werte: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="b2cf6-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="b2cf6-116">name</span><span class="sxs-lookup"><span data-stu-id="b2cf6-116">name</span></span>|<span data-ttu-id="b2cf6-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b2cf6-117">String</span></span>|<span data-ttu-id="b2cf6-118">Stellt den Anzeigenamen einer von [zum](../resources/intune-deviceconfig-windowskioskappbase.md) geerbten App dar.</span><span class="sxs-lookup"><span data-stu-id="b2cf6-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="b2cf6-119">appType</span><span class="sxs-lookup"><span data-stu-id="b2cf6-119">appType</span></span>|[<span data-ttu-id="b2cf6-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="b2cf6-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="b2cf6-121">Der von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)geerbte App-Typ.</span><span class="sxs-lookup"><span data-stu-id="b2cf6-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="b2cf6-122">Mögliche Werte: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="b2cf6-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="b2cf6-123">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="b2cf6-123">appUserModelId</span></span>|<span data-ttu-id="b2cf6-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b2cf6-124">String</span></span>|<span data-ttu-id="b2cf6-125">Dies ist die einzige Anwendungsbenutzer Modell-ID (AUMID), die im Kiosk-Modus verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="b2cf6-125">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="b2cf6-126">appId</span><span class="sxs-lookup"><span data-stu-id="b2cf6-126">appId</span></span>|<span data-ttu-id="b2cf6-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b2cf6-127">String</span></span>|<span data-ttu-id="b2cf6-128">Dies verweist auf eine InTune-APP, die auf die gleichen Zuordnungen wie die Kiosk Konfiguration ausgerichtet sein wird.</span><span class="sxs-lookup"><span data-stu-id="b2cf6-128">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="b2cf6-129">containedAppId</span><span class="sxs-lookup"><span data-stu-id="b2cf6-129">containedAppId</span></span>|<span data-ttu-id="b2cf6-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b2cf6-130">String</span></span>|<span data-ttu-id="b2cf6-131">Dieser Verweis auf eine enthaltene App aus einer InTune-App</span><span class="sxs-lookup"><span data-stu-id="b2cf6-131">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2cf6-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b2cf6-132">Relationships</span></span>
<span data-ttu-id="b2cf6-133">Keine</span><span class="sxs-lookup"><span data-stu-id="b2cf6-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2cf6-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b2cf6-134">JSON Representation</span></span>
<span data-ttu-id="b2cf6-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b2cf6-135">Here is a JSON representation of the resource.</span></span>
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
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```




