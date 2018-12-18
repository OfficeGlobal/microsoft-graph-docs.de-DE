---
title: Ressourcentyp windowsKioskAppBase
description: Die Basisklasse für einen Typ von apps
author: tfitzmac
ms.openlocfilehash: 2afccff07d15fa1f2dfeff6a4ae9029494faa521
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307448"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="dda4c-103">Ressourcentyp windowsKioskAppBase</span><span class="sxs-lookup"><span data-stu-id="dda4c-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="dda4c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dda4c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dda4c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dda4c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dda4c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dda4c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dda4c-107">Die Basisklasse für einen Typ von apps</span><span class="sxs-lookup"><span data-stu-id="dda4c-107">The base class for a type of apps</span></span>
## <a name="properties"></a><span data-ttu-id="dda4c-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dda4c-108">Properties</span></span>
|<span data-ttu-id="dda4c-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dda4c-109">Property</span></span>|<span data-ttu-id="dda4c-110">Typ</span><span class="sxs-lookup"><span data-stu-id="dda4c-110">Type</span></span>|<span data-ttu-id="dda4c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dda4c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dda4c-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="dda4c-112">startLayoutTileSize</span></span>|[<span data-ttu-id="dda4c-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="dda4c-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="dda4c-114">Die app-Kachelgröße für das Layout Start.</span><span class="sxs-lookup"><span data-stu-id="dda4c-114">The app tile size for the start layout.</span></span> <span data-ttu-id="dda4c-115">Mögliche Werte sind: `hidden`, `small`, `medium`, `wide` und `large`.</span><span class="sxs-lookup"><span data-stu-id="dda4c-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="dda4c-116">name</span><span class="sxs-lookup"><span data-stu-id="dda4c-116">name</span></span>|<span data-ttu-id="dda4c-117">String</span><span class="sxs-lookup"><span data-stu-id="dda4c-117">String</span></span>|<span data-ttu-id="dda4c-118">Stellt den Anzeigenamen einer App</span><span class="sxs-lookup"><span data-stu-id="dda4c-118">Represents the friendly name of an app</span></span>|

## <a name="relationships"></a><span data-ttu-id="dda4c-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="dda4c-119">Relationships</span></span>
<span data-ttu-id="dda4c-120">Keine</span><span class="sxs-lookup"><span data-stu-id="dda4c-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dda4c-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dda4c-121">JSON Representation</span></span>
<span data-ttu-id="dda4c-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dda4c-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAppBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAppBase",
  "startLayoutTileSize": "String",
  "name": "String"
}
```





