---
title: Ressourcentyp windowsKioskUWPApp
description: Die Basisklasse für einen Typ von apps
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8719fdd248276a657b96235c592f1bb62607b856
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934912"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="dbaf0-103">Ressourcentyp windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="dbaf0-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="dbaf0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dbaf0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbaf0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dbaf0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dbaf0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dbaf0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dbaf0-107">Die Basisklasse für einen Typ von apps</span><span class="sxs-lookup"><span data-stu-id="dbaf0-107">The base class for a type of apps</span></span>

<span data-ttu-id="dbaf0-108">Erbt vom [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="dbaf0-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dbaf0-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dbaf0-109">Properties</span></span>
|<span data-ttu-id="dbaf0-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dbaf0-110">Property</span></span>|<span data-ttu-id="dbaf0-111">Typ</span><span class="sxs-lookup"><span data-stu-id="dbaf0-111">Type</span></span>|<span data-ttu-id="dbaf0-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dbaf0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbaf0-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="dbaf0-113">startLayoutTileSize</span></span>|[<span data-ttu-id="dbaf0-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="dbaf0-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="dbaf0-115">Die app-Kachelgröße für die Start-Layout Inherited aus [WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="dbaf0-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="dbaf0-116">Mögliche Werte sind: `hidden`, `small`, `medium`, `wide` und `large`.</span><span class="sxs-lookup"><span data-stu-id="dbaf0-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="dbaf0-117">name</span><span class="sxs-lookup"><span data-stu-id="dbaf0-117">name</span></span>|<span data-ttu-id="dbaf0-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dbaf0-118">String</span></span>|<span data-ttu-id="dbaf0-119">Stellt den Anzeigenamen einer App Inherited aus [WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) dar.</span><span class="sxs-lookup"><span data-stu-id="dbaf0-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="dbaf0-120">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="dbaf0-120">appUserModelId</span></span>|<span data-ttu-id="dbaf0-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dbaf0-121">String</span></span>|<span data-ttu-id="dbaf0-122">Dies ist die einzige Anwendung Benutzer Modell ID (AUMID), die Verwendung im Kioskmodus gestartet werden</span><span class="sxs-lookup"><span data-stu-id="dbaf0-122">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="dbaf0-123">appId</span><span class="sxs-lookup"><span data-stu-id="dbaf0-123">appId</span></span>|<span data-ttu-id="dbaf0-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dbaf0-124">String</span></span>|<span data-ttu-id="dbaf0-125">Dies verweist auf eine Intune-App, die Ziel ein, um dieselben Zuweisungen als Kiosk-Konfiguration werden</span><span class="sxs-lookup"><span data-stu-id="dbaf0-125">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="dbaf0-126">containedAppId</span><span class="sxs-lookup"><span data-stu-id="dbaf0-126">containedAppId</span></span>|<span data-ttu-id="dbaf0-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dbaf0-127">String</span></span>|<span data-ttu-id="dbaf0-128">Dies wird auf einer enthaltenen App aus einer Intune App</span><span class="sxs-lookup"><span data-stu-id="dbaf0-128">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="dbaf0-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="dbaf0-129">Relationships</span></span>
<span data-ttu-id="dbaf0-130">Keine</span><span class="sxs-lookup"><span data-stu-id="dbaf0-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dbaf0-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dbaf0-131">JSON Representation</span></span>
<span data-ttu-id="dbaf0-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dbaf0-132">Here is a JSON representation of the resource.</span></span>
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
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```





