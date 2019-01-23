---
title: Ressourcentyp windowsKioskUWPApp
description: Die Basisklasse für einen Typ von apps
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7ba5367721890f02af3b348ad469b15024de4800
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392682"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="df20c-103">Ressourcentyp windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="df20c-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="df20c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="df20c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="df20c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df20c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df20c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="df20c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df20c-107">Die Basisklasse für einen Typ von apps</span><span class="sxs-lookup"><span data-stu-id="df20c-107">The base class for a type of apps</span></span>


<span data-ttu-id="df20c-108">Erbt vom [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="df20c-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="df20c-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="df20c-109">Properties</span></span>
|<span data-ttu-id="df20c-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="df20c-110">Property</span></span>|<span data-ttu-id="df20c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="df20c-111">Type</span></span>|<span data-ttu-id="df20c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df20c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df20c-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="df20c-113">startLayoutTileSize</span></span>|[<span data-ttu-id="df20c-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="df20c-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="df20c-115">Die app-Kachelgröße für die Start-Layout Inherited aus [WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="df20c-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="df20c-116">Mögliche Werte sind: `hidden`, `small`, `medium`, `wide` und `large`.</span><span class="sxs-lookup"><span data-stu-id="df20c-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="df20c-117">name</span><span class="sxs-lookup"><span data-stu-id="df20c-117">name</span></span>|<span data-ttu-id="df20c-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="df20c-118">String</span></span>|<span data-ttu-id="df20c-119">Stellt den Anzeigenamen einer App Inherited aus [WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) dar.</span><span class="sxs-lookup"><span data-stu-id="df20c-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="df20c-120">der appType</span><span class="sxs-lookup"><span data-stu-id="df20c-120">appType</span></span>|[<span data-ttu-id="df20c-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="df20c-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="df20c-122">Der app-Typ Inherited aus [WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="df20c-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="df20c-123">Mögliche Werte: sind `unknown`, `store`, `desktop` und `aumId`.</span><span class="sxs-lookup"><span data-stu-id="df20c-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="df20c-124">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="df20c-124">appUserModelId</span></span>|<span data-ttu-id="df20c-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="df20c-125">String</span></span>|<span data-ttu-id="df20c-126">Dies ist die einzige Anwendung Benutzer Modell ID (AUMID), die Verwendung im Kioskmodus gestartet werden</span><span class="sxs-lookup"><span data-stu-id="df20c-126">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="df20c-127">appId</span><span class="sxs-lookup"><span data-stu-id="df20c-127">appId</span></span>|<span data-ttu-id="df20c-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="df20c-128">String</span></span>|<span data-ttu-id="df20c-129">Dies verweist auf eine Intune-App, die Ziel ein, um dieselben Zuweisungen als Kiosk-Konfiguration werden</span><span class="sxs-lookup"><span data-stu-id="df20c-129">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="df20c-130">containedAppId</span><span class="sxs-lookup"><span data-stu-id="df20c-130">containedAppId</span></span>|<span data-ttu-id="df20c-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="df20c-131">String</span></span>|<span data-ttu-id="df20c-132">Dies wird auf einer enthaltenen App aus einer Intune App</span><span class="sxs-lookup"><span data-stu-id="df20c-132">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="df20c-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="df20c-133">Relationships</span></span>
<span data-ttu-id="df20c-134">Keine</span><span class="sxs-lookup"><span data-stu-id="df20c-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df20c-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="df20c-135">JSON Representation</span></span>
<span data-ttu-id="df20c-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="df20c-136">Here is a JSON representation of the resource.</span></span>
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




