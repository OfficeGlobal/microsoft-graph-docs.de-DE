---
title: iPv4Range-Ressourcentyp
description: Definition des IPv4-Umfangs.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 521c27396c483ba07cc39aec583dd3e610da267d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160515"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="399eb-103">iPv4Range-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="399eb-103">iPv4Range resource type</span></span>

> <span data-ttu-id="399eb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="399eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="399eb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="399eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="399eb-106">Definition des IPv4-Umfangs.</span><span class="sxs-lookup"><span data-stu-id="399eb-106">IPv4 Range definition.</span></span>


<span data-ttu-id="399eb-107">Erbt von [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="399eb-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="399eb-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="399eb-108">Properties</span></span>
|<span data-ttu-id="399eb-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="399eb-109">Property</span></span>|<span data-ttu-id="399eb-110">Typ</span><span class="sxs-lookup"><span data-stu-id="399eb-110">Type</span></span>|<span data-ttu-id="399eb-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="399eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="399eb-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="399eb-112">lowerAddress</span></span>|<span data-ttu-id="399eb-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="399eb-113">String</span></span>|<span data-ttu-id="399eb-114">Niedrigere Adresse.</span><span class="sxs-lookup"><span data-stu-id="399eb-114">Lower address.</span></span>|
|<span data-ttu-id="399eb-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="399eb-115">upperAddress</span></span>|<span data-ttu-id="399eb-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="399eb-116">String</span></span>|<span data-ttu-id="399eb-117">Obere Adresse.</span><span class="sxs-lookup"><span data-stu-id="399eb-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="399eb-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="399eb-118">Relationships</span></span>
<span data-ttu-id="399eb-119">Keine</span><span class="sxs-lookup"><span data-stu-id="399eb-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="399eb-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="399eb-120">JSON Representation</span></span>
<span data-ttu-id="399eb-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="399eb-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```




