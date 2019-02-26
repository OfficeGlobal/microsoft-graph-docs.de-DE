---
title: deliveryOptimizationGroupIdCustom-Ressourcentyp
description: Benutzerdefinierter Gruppen-ID-Typ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec3b00920d0ead3df5fe694e110825615f449ef4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177973"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="c3ba8-103">deliveryOptimizationGroupIdCustom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c3ba8-103">deliveryOptimizationGroupIdCustom resource type</span></span>

> <span data-ttu-id="c3ba8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c3ba8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3ba8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c3ba8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3ba8-106">Benutzerdefinierter Gruppen-ID-Typ</span><span class="sxs-lookup"><span data-stu-id="c3ba8-106">Custom group id type</span></span>


<span data-ttu-id="c3ba8-107">Erbt von [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="c3ba8-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c3ba8-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c3ba8-108">Properties</span></span>
|<span data-ttu-id="c3ba8-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c3ba8-109">Property</span></span>|<span data-ttu-id="c3ba8-110">Typ</span><span class="sxs-lookup"><span data-stu-id="c3ba8-110">Type</span></span>|<span data-ttu-id="c3ba8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c3ba8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3ba8-112">groupIdCustom</span><span class="sxs-lookup"><span data-stu-id="c3ba8-112">groupIdCustom</span></span>|<span data-ttu-id="c3ba8-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c3ba8-113">String</span></span>|<span data-ttu-id="c3ba8-114">Gibt eine beliebige Gruppen-ID an, zu der das Gerät gehört.</span><span class="sxs-lookup"><span data-stu-id="c3ba8-114">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3ba8-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c3ba8-115">Relationships</span></span>
<span data-ttu-id="c3ba8-116">Keine</span><span class="sxs-lookup"><span data-stu-id="c3ba8-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3ba8-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c3ba8-117">JSON Representation</span></span>
<span data-ttu-id="c3ba8-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c3ba8-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdCustom",
  "groupIdCustom": "String"
}
```




