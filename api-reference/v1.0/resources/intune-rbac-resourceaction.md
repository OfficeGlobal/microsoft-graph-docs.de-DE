---
title: resourceAction-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a48d09d8aeadc9a5d60559d25a4bdcc322d10f21
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262181"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="b1ce2-103">resourceAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b1ce2-103">resourceAction resource type</span></span>

> <span data-ttu-id="b1ce2-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b1ce2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1ce2-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b1ce2-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b1ce2-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b1ce2-106">Properties</span></span>
|<span data-ttu-id="b1ce2-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b1ce2-107">Property</span></span>|<span data-ttu-id="b1ce2-108">Typ</span><span class="sxs-lookup"><span data-stu-id="b1ce2-108">Type</span></span>|<span data-ttu-id="b1ce2-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1ce2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1ce2-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="b1ce2-110">allowedResourceActions</span></span>|<span data-ttu-id="b1ce2-111">String collection</span><span class="sxs-lookup"><span data-stu-id="b1ce2-111">String collection</span></span>|<span data-ttu-id="b1ce2-112">Zulässige Aktionen</span><span class="sxs-lookup"><span data-stu-id="b1ce2-112">Allowed Actions</span></span>|
|<span data-ttu-id="b1ce2-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="b1ce2-113">notAllowedResourceActions</span></span>|<span data-ttu-id="b1ce2-114">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b1ce2-114">String collection</span></span>|<span data-ttu-id="b1ce2-115">Nicht zulässige Aktionen</span><span class="sxs-lookup"><span data-stu-id="b1ce2-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1ce2-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b1ce2-116">Relationships</span></span>
<span data-ttu-id="b1ce2-117">Keine</span><span class="sxs-lookup"><span data-stu-id="b1ce2-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1ce2-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b1ce2-118">JSON Representation</span></span>
<span data-ttu-id="b1ce2-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b1ce2-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```



