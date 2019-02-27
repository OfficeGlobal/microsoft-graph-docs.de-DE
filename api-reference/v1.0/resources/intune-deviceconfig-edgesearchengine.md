---
title: edgeSearchEngine-Ressourcentyp
description: Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6867dd6b2243541b193b8b741924487f16ff61c5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254471"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="9526d-103">edgeSearchEngine-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9526d-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="9526d-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9526d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9526d-105">Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="9526d-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="9526d-106">Erbt von [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="9526d-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9526d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9526d-107">Properties</span></span>
|<span data-ttu-id="9526d-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9526d-108">Property</span></span>|<span data-ttu-id="9526d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9526d-109">Type</span></span>|<span data-ttu-id="9526d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9526d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9526d-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="9526d-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="9526d-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="9526d-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="9526d-113">Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="9526d-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="9526d-114">Mögliche Werte: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="9526d-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9526d-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9526d-115">Relationships</span></span>
<span data-ttu-id="9526d-116">Keine</span><span class="sxs-lookup"><span data-stu-id="9526d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9526d-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9526d-117">JSON Representation</span></span>
<span data-ttu-id="9526d-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9526d-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```



