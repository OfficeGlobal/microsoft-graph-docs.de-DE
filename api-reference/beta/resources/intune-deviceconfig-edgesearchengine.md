---
title: edgeSearchEngine-Ressourcentyp
description: Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b59fa163fe453d4f26dd71afa24edf9ac37d9d41
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953238"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="df35a-103">edgeSearchEngine-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="df35a-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="df35a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="df35a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df35a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df35a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df35a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="df35a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df35a-107">Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="df35a-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="df35a-108">Erbt von [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="df35a-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="df35a-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="df35a-109">Properties</span></span>
|<span data-ttu-id="df35a-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="df35a-110">Property</span></span>|<span data-ttu-id="df35a-111">Typ</span><span class="sxs-lookup"><span data-stu-id="df35a-111">Type</span></span>|<span data-ttu-id="df35a-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df35a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df35a-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="df35a-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="df35a-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="df35a-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="df35a-115">Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="df35a-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="df35a-116">Mögliche Werte: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="df35a-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df35a-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="df35a-117">Relationships</span></span>
<span data-ttu-id="df35a-118">Keine</span><span class="sxs-lookup"><span data-stu-id="df35a-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="df35a-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="df35a-119">JSON Representation</span></span>
<span data-ttu-id="df35a-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="df35a-120">Here is a JSON representation of the resource.</span></span>
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





