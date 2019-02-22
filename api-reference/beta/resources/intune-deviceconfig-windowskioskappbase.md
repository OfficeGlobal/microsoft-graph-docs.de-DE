---
title: Zum-Ressourcentyp
description: Die Basisklasse für eine Art von apps
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0247febfbeebe7fc047df4bb14a9d421b79bf01
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145297"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="8e796-103">Zum-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8e796-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="8e796-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8e796-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e796-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8e796-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e796-106">Die Basisklasse für eine Art von apps</span><span class="sxs-lookup"><span data-stu-id="8e796-106">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="8e796-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8e796-107">Properties</span></span>
|<span data-ttu-id="8e796-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e796-108">Property</span></span>|<span data-ttu-id="8e796-109">Typ</span><span class="sxs-lookup"><span data-stu-id="8e796-109">Type</span></span>|<span data-ttu-id="8e796-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e796-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e796-111">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="8e796-111">startLayoutTileSize</span></span>|[<span data-ttu-id="8e796-112">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="8e796-112">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="8e796-113">Die Größe der APP-Kachel für das Start Layout.</span><span class="sxs-lookup"><span data-stu-id="8e796-113">The app tile size for the start layout.</span></span> <span data-ttu-id="8e796-114">Mögliche Werte: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="8e796-114">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="8e796-115">name</span><span class="sxs-lookup"><span data-stu-id="8e796-115">name</span></span>|<span data-ttu-id="8e796-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8e796-116">String</span></span>|<span data-ttu-id="8e796-117">Stellt den Anzeigenamen einer APP dar.</span><span class="sxs-lookup"><span data-stu-id="8e796-117">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="8e796-118">appType</span><span class="sxs-lookup"><span data-stu-id="8e796-118">appType</span></span>|[<span data-ttu-id="8e796-119">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="8e796-119">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="8e796-120">Der APP-Typ.</span><span class="sxs-lookup"><span data-stu-id="8e796-120">The app type.</span></span> <span data-ttu-id="8e796-121">Mögliche Werte: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="8e796-121">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e796-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8e796-122">Relationships</span></span>
<span data-ttu-id="8e796-123">Keine</span><span class="sxs-lookup"><span data-stu-id="8e796-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e796-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8e796-124">JSON Representation</span></span>
<span data-ttu-id="8e796-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8e796-125">Here is a JSON representation of the resource.</span></span>
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




