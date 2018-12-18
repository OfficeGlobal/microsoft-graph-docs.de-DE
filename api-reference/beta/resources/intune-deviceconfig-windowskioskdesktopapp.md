---
title: Ressourcentyp windowsKioskDesktopApp
description: Die Basisklasse für einen Typ von apps
author: tfitzmac
ms.openlocfilehash: a5ef4000b66f15f5951b49a152d25df30167004d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344520"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="8230f-103">Ressourcentyp windowsKioskDesktopApp</span><span class="sxs-lookup"><span data-stu-id="8230f-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="8230f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8230f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8230f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8230f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8230f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8230f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8230f-107">Die Basisklasse für einen Typ von apps</span><span class="sxs-lookup"><span data-stu-id="8230f-107">The base class for a type of apps</span></span>

<span data-ttu-id="8230f-108">Erbt vom [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="8230f-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8230f-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8230f-109">Properties</span></span>
|<span data-ttu-id="8230f-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8230f-110">Property</span></span>|<span data-ttu-id="8230f-111">Typ</span><span class="sxs-lookup"><span data-stu-id="8230f-111">Type</span></span>|<span data-ttu-id="8230f-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8230f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8230f-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="8230f-113">startLayoutTileSize</span></span>|[<span data-ttu-id="8230f-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="8230f-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="8230f-115">Die app-Kachelgröße für die Start-Layout Inherited aus [WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="8230f-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="8230f-116">Mögliche Werte sind: `hidden`, `small`, `medium`, `wide` und `large`.</span><span class="sxs-lookup"><span data-stu-id="8230f-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="8230f-117">name</span><span class="sxs-lookup"><span data-stu-id="8230f-117">name</span></span>|<span data-ttu-id="8230f-118">String</span><span class="sxs-lookup"><span data-stu-id="8230f-118">String</span></span>|<span data-ttu-id="8230f-119">Stellt den Anzeigenamen einer App Inherited aus [WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) dar.</span><span class="sxs-lookup"><span data-stu-id="8230f-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="8230f-120">Pfad</span><span class="sxs-lookup"><span data-stu-id="8230f-120">path</span></span>|<span data-ttu-id="8230f-121">String</span><span class="sxs-lookup"><span data-stu-id="8230f-121">String</span></span>|<span data-ttu-id="8230f-122">Definieren Sie den Pfad einer desktop-App</span><span class="sxs-lookup"><span data-stu-id="8230f-122">Define the path of a desktop app</span></span>|
|<span data-ttu-id="8230f-123">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="8230f-123">desktopApplicationId</span></span>|<span data-ttu-id="8230f-124">String</span><span class="sxs-lookup"><span data-stu-id="8230f-124">String</span></span>|<span data-ttu-id="8230f-125">Definieren der DesktopApplicationID der app</span><span class="sxs-lookup"><span data-stu-id="8230f-125">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="8230f-126">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="8230f-126">desktopApplicationLinkPath</span></span>|<span data-ttu-id="8230f-127">String</span><span class="sxs-lookup"><span data-stu-id="8230f-127">String</span></span>|<span data-ttu-id="8230f-128">Definieren der DesktopApplicationLinkPath der app</span><span class="sxs-lookup"><span data-stu-id="8230f-128">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="8230f-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8230f-129">Relationships</span></span>
<span data-ttu-id="8230f-130">Keine</span><span class="sxs-lookup"><span data-stu-id="8230f-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8230f-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8230f-131">JSON Representation</span></span>
<span data-ttu-id="8230f-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8230f-132">Here is a JSON representation of the resource.</span></span>
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
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```





