---
title: Ressourcentyp windowsKioskAppBase
description: Die Basisklasse für einen Typ von apps
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8ca86969eb32a1a1d129fb5ba4cd48bbb04ffd78
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407144"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="30c17-103">Ressourcentyp windowsKioskAppBase</span><span class="sxs-lookup"><span data-stu-id="30c17-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="30c17-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="30c17-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="30c17-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="30c17-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30c17-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="30c17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30c17-107">Die Basisklasse für einen Typ von apps</span><span class="sxs-lookup"><span data-stu-id="30c17-107">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="30c17-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="30c17-108">Properties</span></span>
|<span data-ttu-id="30c17-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="30c17-109">Property</span></span>|<span data-ttu-id="30c17-110">Typ</span><span class="sxs-lookup"><span data-stu-id="30c17-110">Type</span></span>|<span data-ttu-id="30c17-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30c17-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30c17-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="30c17-112">startLayoutTileSize</span></span>|[<span data-ttu-id="30c17-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="30c17-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="30c17-114">Die app-Kachelgröße für das Layout Start.</span><span class="sxs-lookup"><span data-stu-id="30c17-114">The app tile size for the start layout.</span></span> <span data-ttu-id="30c17-115">Mögliche Werte sind: `hidden`, `small`, `medium`, `wide` und `large`.</span><span class="sxs-lookup"><span data-stu-id="30c17-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="30c17-116">name</span><span class="sxs-lookup"><span data-stu-id="30c17-116">name</span></span>|<span data-ttu-id="30c17-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="30c17-117">String</span></span>|<span data-ttu-id="30c17-118">Stellt den Anzeigenamen einer App</span><span class="sxs-lookup"><span data-stu-id="30c17-118">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="30c17-119">der appType</span><span class="sxs-lookup"><span data-stu-id="30c17-119">appType</span></span>|[<span data-ttu-id="30c17-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="30c17-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="30c17-121">Der app-Typ.</span><span class="sxs-lookup"><span data-stu-id="30c17-121">The app type.</span></span> <span data-ttu-id="30c17-122">Mögliche Werte: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="30c17-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30c17-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="30c17-123">Relationships</span></span>
<span data-ttu-id="30c17-124">Keine</span><span class="sxs-lookup"><span data-stu-id="30c17-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="30c17-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="30c17-125">JSON Representation</span></span>
<span data-ttu-id="30c17-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="30c17-126">Here is a JSON representation of the resource.</span></span>
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
  "appType": "String"
}
```




