---
title: iPv6Range-Ressourcentyp
description: IPv6-Range-Definition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f171a8ebb28d15e78a30bf542c37a163f0d097f0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258989"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="e10aa-103">iPv6Range-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e10aa-103">iPv6Range resource type</span></span>

> <span data-ttu-id="e10aa-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e10aa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e10aa-105">IPv6-Range-Definition.</span><span class="sxs-lookup"><span data-stu-id="e10aa-105">IPv6 Range definition.</span></span>


<span data-ttu-id="e10aa-106">Erbt von [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="e10aa-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e10aa-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e10aa-107">Properties</span></span>
|<span data-ttu-id="e10aa-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e10aa-108">Property</span></span>|<span data-ttu-id="e10aa-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e10aa-109">Type</span></span>|<span data-ttu-id="e10aa-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e10aa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e10aa-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="e10aa-111">lowerAddress</span></span>|<span data-ttu-id="e10aa-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e10aa-112">String</span></span>|<span data-ttu-id="e10aa-113">Niedrigere Adresse</span><span class="sxs-lookup"><span data-stu-id="e10aa-113">Lower address</span></span>|
|<span data-ttu-id="e10aa-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="e10aa-114">upperAddress</span></span>|<span data-ttu-id="e10aa-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e10aa-115">String</span></span>|<span data-ttu-id="e10aa-116">Obere Adresse</span><span class="sxs-lookup"><span data-stu-id="e10aa-116">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="e10aa-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e10aa-117">Relationships</span></span>
<span data-ttu-id="e10aa-118">Keine</span><span class="sxs-lookup"><span data-stu-id="e10aa-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e10aa-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e10aa-119">JSON Representation</span></span>
<span data-ttu-id="e10aa-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e10aa-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



