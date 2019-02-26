---
title: edgeSearchEngine-Ressourcentyp
description: Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75c5864a9f9d78b9ea9555c31ae1bc2baec28e49
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163217"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="14cbe-103">edgeSearchEngine-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="14cbe-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="14cbe-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="14cbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14cbe-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="14cbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14cbe-106">Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="14cbe-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="14cbe-107">Erbt von [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="14cbe-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="14cbe-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="14cbe-108">Properties</span></span>
|<span data-ttu-id="14cbe-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="14cbe-109">Property</span></span>|<span data-ttu-id="14cbe-110">Typ</span><span class="sxs-lookup"><span data-stu-id="14cbe-110">Type</span></span>|<span data-ttu-id="14cbe-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14cbe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14cbe-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="14cbe-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="14cbe-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="14cbe-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="14cbe-114">Ermöglicht es IT-Administratoren, eine vordefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="14cbe-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="14cbe-115">Mögliche Werte: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="14cbe-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14cbe-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="14cbe-116">Relationships</span></span>
<span data-ttu-id="14cbe-117">Keine</span><span class="sxs-lookup"><span data-stu-id="14cbe-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14cbe-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="14cbe-118">JSON Representation</span></span>
<span data-ttu-id="14cbe-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="14cbe-119">Here is a JSON representation of the resource.</span></span>
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




