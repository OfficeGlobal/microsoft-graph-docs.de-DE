---
title: edgeSearchEngine-Ressourcentyp
description: Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.
author: tfitzmac
ms.openlocfilehash: 0c49780ddd7d2174116f7a0821fa98681d3e5d2a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339732"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="bd4b1-103">edgeSearchEngine-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bd4b1-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="bd4b1-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bd4b1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd4b1-105">Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="bd4b1-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="bd4b1-106">Erbt von [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="bd4b1-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bd4b1-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bd4b1-107">Properties</span></span>
|<span data-ttu-id="bd4b1-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd4b1-108">Property</span></span>|<span data-ttu-id="bd4b1-109">Typ</span><span class="sxs-lookup"><span data-stu-id="bd4b1-109">Type</span></span>|<span data-ttu-id="bd4b1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd4b1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd4b1-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="bd4b1-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="bd4b1-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="bd4b1-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="bd4b1-113">Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="bd4b1-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="bd4b1-114">Mögliche Werte: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="bd4b1-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd4b1-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bd4b1-115">Relationships</span></span>
<span data-ttu-id="bd4b1-116">Keine</span><span class="sxs-lookup"><span data-stu-id="bd4b1-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bd4b1-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bd4b1-117">JSON Representation</span></span>
<span data-ttu-id="bd4b1-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bd4b1-118">Here is a JSON representation of the resource.</span></span>
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



