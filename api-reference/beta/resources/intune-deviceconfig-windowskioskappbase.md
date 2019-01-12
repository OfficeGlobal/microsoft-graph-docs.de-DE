---
title: Ressourcentyp windowsKioskAppBase
description: Die Basisklasse für einen Typ von apps
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9b13807fdb0319b3c9a15248fa2d50ffc46ac164
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977024"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="06e01-103">Ressourcentyp windowsKioskAppBase</span><span class="sxs-lookup"><span data-stu-id="06e01-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="06e01-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="06e01-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06e01-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="06e01-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06e01-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="06e01-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06e01-107">Die Basisklasse für einen Typ von apps</span><span class="sxs-lookup"><span data-stu-id="06e01-107">The base class for a type of apps</span></span>
## <a name="properties"></a><span data-ttu-id="06e01-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="06e01-108">Properties</span></span>
|<span data-ttu-id="06e01-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="06e01-109">Property</span></span>|<span data-ttu-id="06e01-110">Typ</span><span class="sxs-lookup"><span data-stu-id="06e01-110">Type</span></span>|<span data-ttu-id="06e01-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06e01-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06e01-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="06e01-112">startLayoutTileSize</span></span>|[<span data-ttu-id="06e01-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="06e01-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="06e01-114">Die app-Kachelgröße für das Layout Start.</span><span class="sxs-lookup"><span data-stu-id="06e01-114">The app tile size for the start layout.</span></span> <span data-ttu-id="06e01-115">Mögliche Werte sind: `hidden`, `small`, `medium`, `wide` und `large`.</span><span class="sxs-lookup"><span data-stu-id="06e01-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="06e01-116">name</span><span class="sxs-lookup"><span data-stu-id="06e01-116">name</span></span>|<span data-ttu-id="06e01-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06e01-117">String</span></span>|<span data-ttu-id="06e01-118">Stellt den Anzeigenamen einer App</span><span class="sxs-lookup"><span data-stu-id="06e01-118">Represents the friendly name of an app</span></span>|

## <a name="relationships"></a><span data-ttu-id="06e01-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="06e01-119">Relationships</span></span>
<span data-ttu-id="06e01-120">Keine</span><span class="sxs-lookup"><span data-stu-id="06e01-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="06e01-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="06e01-121">JSON Representation</span></span>
<span data-ttu-id="06e01-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="06e01-122">Here is a JSON representation of the resource.</span></span>
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





