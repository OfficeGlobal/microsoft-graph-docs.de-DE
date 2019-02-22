---
title: KeyValue-Ressourcentyp
description: Schlüsselwert Definition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 597f6d2101e4549336693f1cff7ce64199b46287
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155496"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="6f7b4-103">KeyValue-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6f7b4-103">keyValue resource type</span></span>

> <span data-ttu-id="6f7b4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f7b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f7b4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6f7b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f7b4-106">Schlüsselwert Definition.</span><span class="sxs-lookup"><span data-stu-id="6f7b4-106">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="6f7b4-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6f7b4-107">Properties</span></span>
|<span data-ttu-id="6f7b4-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6f7b4-108">Property</span></span>|<span data-ttu-id="6f7b4-109">Typ</span><span class="sxs-lookup"><span data-stu-id="6f7b4-109">Type</span></span>|<span data-ttu-id="6f7b4-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f7b4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f7b4-111">Key</span><span class="sxs-lookup"><span data-stu-id="6f7b4-111">key</span></span>|<span data-ttu-id="6f7b4-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f7b4-112">String</span></span>|<span data-ttu-id="6f7b4-113">Key.</span><span class="sxs-lookup"><span data-stu-id="6f7b4-113">Key.</span></span>|
|<span data-ttu-id="6f7b4-114">Wert</span><span class="sxs-lookup"><span data-stu-id="6f7b4-114">value</span></span>|<span data-ttu-id="6f7b4-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f7b4-115">String</span></span>|<span data-ttu-id="6f7b4-116">Wert.</span><span class="sxs-lookup"><span data-stu-id="6f7b4-116">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f7b4-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6f7b4-117">Relationships</span></span>
<span data-ttu-id="6f7b4-118">Keine</span><span class="sxs-lookup"><span data-stu-id="6f7b4-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f7b4-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6f7b4-119">JSON Representation</span></span>
<span data-ttu-id="6f7b4-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6f7b4-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```




