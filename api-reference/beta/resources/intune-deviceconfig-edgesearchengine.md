---
title: edgeSearchEngine-Ressourcentyp
description: Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b868be9ff34e85516e34040cb3ccb6f0efb95cb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402370"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="ad633-103">edgeSearchEngine-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ad633-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="ad633-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ad633-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ad633-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ad633-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad633-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ad633-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad633-107">Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="ad633-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="ad633-108">Erbt von [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="ad633-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ad633-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ad633-109">Properties</span></span>
|<span data-ttu-id="ad633-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ad633-110">Property</span></span>|<span data-ttu-id="ad633-111">Typ</span><span class="sxs-lookup"><span data-stu-id="ad633-111">Type</span></span>|<span data-ttu-id="ad633-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ad633-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad633-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="ad633-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="ad633-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="ad633-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="ad633-115">Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="ad633-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="ad633-116">Mögliche Werte: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="ad633-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad633-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ad633-117">Relationships</span></span>
<span data-ttu-id="ad633-118">Keine</span><span class="sxs-lookup"><span data-stu-id="ad633-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad633-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ad633-119">JSON Representation</span></span>
<span data-ttu-id="ad633-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ad633-120">Here is a JSON representation of the resource.</span></span>
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




