---
title: Ressourcentyp windowsKioskDesktopApp
description: Die Basisklasse für einen Typ von apps
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 831ed86da24791cde549687ecaff42cabc29a99e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415306"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="6ffd8-103">Ressourcentyp windowsKioskDesktopApp</span><span class="sxs-lookup"><span data-stu-id="6ffd8-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="6ffd8-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6ffd8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6ffd8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6ffd8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ffd8-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6ffd8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ffd8-107">Die Basisklasse für einen Typ von apps</span><span class="sxs-lookup"><span data-stu-id="6ffd8-107">The base class for a type of apps</span></span>


<span data-ttu-id="6ffd8-108">Erbt vom [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="6ffd8-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6ffd8-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6ffd8-109">Properties</span></span>
|<span data-ttu-id="6ffd8-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6ffd8-110">Property</span></span>|<span data-ttu-id="6ffd8-111">Typ</span><span class="sxs-lookup"><span data-stu-id="6ffd8-111">Type</span></span>|<span data-ttu-id="6ffd8-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ffd8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ffd8-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="6ffd8-113">startLayoutTileSize</span></span>|[<span data-ttu-id="6ffd8-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="6ffd8-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="6ffd8-115">Die app-Kachelgröße für die Start-Layout Inherited aus [WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="6ffd8-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="6ffd8-116">Mögliche Werte sind: `hidden`, `small`, `medium`, `wide` und `large`.</span><span class="sxs-lookup"><span data-stu-id="6ffd8-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="6ffd8-117">name</span><span class="sxs-lookup"><span data-stu-id="6ffd8-117">name</span></span>|<span data-ttu-id="6ffd8-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6ffd8-118">String</span></span>|<span data-ttu-id="6ffd8-119">Stellt den Anzeigenamen einer App Inherited aus [WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) dar.</span><span class="sxs-lookup"><span data-stu-id="6ffd8-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="6ffd8-120">der appType</span><span class="sxs-lookup"><span data-stu-id="6ffd8-120">appType</span></span>|[<span data-ttu-id="6ffd8-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="6ffd8-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="6ffd8-122">Der app-Typ Inherited aus [WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="6ffd8-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="6ffd8-123">Mögliche Werte: sind `unknown`, `store`, `desktop` und `aumId`.</span><span class="sxs-lookup"><span data-stu-id="6ffd8-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="6ffd8-124">Pfad</span><span class="sxs-lookup"><span data-stu-id="6ffd8-124">path</span></span>|<span data-ttu-id="6ffd8-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6ffd8-125">String</span></span>|<span data-ttu-id="6ffd8-126">Definieren Sie den Pfad einer desktop-App</span><span class="sxs-lookup"><span data-stu-id="6ffd8-126">Define the path of a desktop app</span></span>|
|<span data-ttu-id="6ffd8-127">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="6ffd8-127">desktopApplicationId</span></span>|<span data-ttu-id="6ffd8-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6ffd8-128">String</span></span>|<span data-ttu-id="6ffd8-129">Definieren der DesktopApplicationID der app</span><span class="sxs-lookup"><span data-stu-id="6ffd8-129">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="6ffd8-130">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="6ffd8-130">desktopApplicationLinkPath</span></span>|<span data-ttu-id="6ffd8-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6ffd8-131">String</span></span>|<span data-ttu-id="6ffd8-132">Definieren der DesktopApplicationLinkPath der app</span><span class="sxs-lookup"><span data-stu-id="6ffd8-132">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ffd8-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6ffd8-133">Relationships</span></span>
<span data-ttu-id="6ffd8-134">Keine</span><span class="sxs-lookup"><span data-stu-id="6ffd8-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ffd8-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6ffd8-135">JSON Representation</span></span>
<span data-ttu-id="6ffd8-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6ffd8-136">Here is a JSON representation of the resource.</span></span>
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




