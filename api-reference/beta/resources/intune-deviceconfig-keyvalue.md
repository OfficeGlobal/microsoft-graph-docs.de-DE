---
title: KeyValue Ressourcentyp
description: Definition von Schlüssel-Wert.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e3133962d9f6bfb5f5363dd6d6cbd4b5ef2ea202
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406815"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="b6d01-103">KeyValue Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b6d01-103">keyValue resource type</span></span>

> <span data-ttu-id="b6d01-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b6d01-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b6d01-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b6d01-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6d01-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b6d01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6d01-107">Definition von Schlüssel-Wert.</span><span class="sxs-lookup"><span data-stu-id="b6d01-107">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="b6d01-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b6d01-108">Properties</span></span>
|<span data-ttu-id="b6d01-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b6d01-109">Property</span></span>|<span data-ttu-id="b6d01-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b6d01-110">Type</span></span>|<span data-ttu-id="b6d01-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b6d01-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6d01-112">Key</span><span class="sxs-lookup"><span data-stu-id="b6d01-112">key</span></span>|<span data-ttu-id="b6d01-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b6d01-113">String</span></span>|<span data-ttu-id="b6d01-114">Key.</span><span class="sxs-lookup"><span data-stu-id="b6d01-114">Key.</span></span>|
|<span data-ttu-id="b6d01-115">Wert</span><span class="sxs-lookup"><span data-stu-id="b6d01-115">value</span></span>|<span data-ttu-id="b6d01-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b6d01-116">String</span></span>|<span data-ttu-id="b6d01-117">Wert.</span><span class="sxs-lookup"><span data-stu-id="b6d01-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6d01-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b6d01-118">Relationships</span></span>
<span data-ttu-id="b6d01-119">Keine</span><span class="sxs-lookup"><span data-stu-id="b6d01-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6d01-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b6d01-120">JSON Representation</span></span>
<span data-ttu-id="b6d01-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b6d01-121">Here is a JSON representation of the resource.</span></span>
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




