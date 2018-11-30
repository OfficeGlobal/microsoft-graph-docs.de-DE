---
title: edgeSearchEngine-Ressourcentyp
description: Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.
ms.openlocfilehash: 51f947911e73927816eb4f1150cab36cba904f58
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058166"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="7076f-103">edgeSearchEngine-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7076f-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="7076f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7076f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7076f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7076f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7076f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7076f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7076f-107">Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="7076f-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="7076f-108">Erbt von [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="7076f-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7076f-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7076f-109">Properties</span></span>
|<span data-ttu-id="7076f-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7076f-110">Property</span></span>|<span data-ttu-id="7076f-111">Typ</span><span class="sxs-lookup"><span data-stu-id="7076f-111">Type</span></span>|<span data-ttu-id="7076f-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7076f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7076f-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="7076f-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="7076f-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="7076f-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="7076f-115">Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="7076f-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="7076f-116">Mögliche Werte: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="7076f-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7076f-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7076f-117">Relationships</span></span>
<span data-ttu-id="7076f-118">Keine</span><span class="sxs-lookup"><span data-stu-id="7076f-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7076f-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7076f-119">JSON Representation</span></span>
<span data-ttu-id="7076f-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7076f-120">Here is a JSON representation of the resource.</span></span>
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





