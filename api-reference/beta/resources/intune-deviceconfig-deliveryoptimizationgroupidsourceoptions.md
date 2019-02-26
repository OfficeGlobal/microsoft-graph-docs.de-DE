---
title: deliveryOptimizationGroupIdSourceOptions-Ressourcentyp
description: Typ der Gruppen-ID-Optionen
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d54a98bef3b9c0e0517b426332b8d3223e904c8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177854"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="8c448-103">deliveryOptimizationGroupIdSourceOptions-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8c448-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

> <span data-ttu-id="8c448-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8c448-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c448-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8c448-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c448-106">Typ der Gruppen-ID-Optionen</span><span class="sxs-lookup"><span data-stu-id="8c448-106">Group id options type</span></span>


<span data-ttu-id="8c448-107">Erbt von [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="8c448-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8c448-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8c448-108">Properties</span></span>
|<span data-ttu-id="8c448-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8c448-109">Property</span></span>|<span data-ttu-id="8c448-110">Typ</span><span class="sxs-lookup"><span data-stu-id="8c448-110">Type</span></span>|<span data-ttu-id="8c448-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c448-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c448-112">groupIdSourceOption</span><span class="sxs-lookup"><span data-stu-id="8c448-112">groupIdSourceOption</span></span>|[<span data-ttu-id="8c448-113">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="8c448-113">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="8c448-114">Legen Sie diese Richtlinie fest, um die Peer Auswahl auf eine bestimmte Quelle zu beschränken.</span><span class="sxs-lookup"><span data-stu-id="8c448-114">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="8c448-115">Mögliche Werte: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span><span class="sxs-lookup"><span data-stu-id="8c448-115">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c448-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8c448-116">Relationships</span></span>
<span data-ttu-id="8c448-117">Keine</span><span class="sxs-lookup"><span data-stu-id="8c448-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c448-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8c448-118">JSON Representation</span></span>
<span data-ttu-id="8c448-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8c448-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSourceOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdSourceOptions",
  "groupIdSourceOption": "String"
}
```




