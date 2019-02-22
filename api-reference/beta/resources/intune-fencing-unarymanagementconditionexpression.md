---
title: unaryManagementConditionExpression-Ressourcentyp
description: Ein Ausdruck der Verwaltungsbedingung, der mit einer unären Operation ausgewertet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9802cb8162973ecdaa387a29c70d1baa7aec4b8b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164218"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="e9932-103">unaryManagementConditionExpression-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e9932-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="e9932-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e9932-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9932-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e9932-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9932-106">Ein Ausdruck der Verwaltungsbedingung, der mit einer unären Operation ausgewertet wird.</span><span class="sxs-lookup"><span data-stu-id="e9932-106">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="e9932-107">Erbt von [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="e9932-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e9932-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e9932-108">Properties</span></span>
|<span data-ttu-id="e9932-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e9932-109">Property</span></span>|<span data-ttu-id="e9932-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e9932-110">Type</span></span>|<span data-ttu-id="e9932-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9932-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9932-112">operator</span><span class="sxs-lookup"><span data-stu-id="e9932-112">operator</span></span>|[<span data-ttu-id="e9932-113">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="e9932-113">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="e9932-114">Der Operator, der bei der Auswertung des unären Vorgangs verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="e9932-114">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="e9932-115">Mögliche Werte sind: `not`.</span><span class="sxs-lookup"><span data-stu-id="e9932-115">Possible values are: `not`.</span></span>|
|<span data-ttu-id="e9932-116">Operand</span><span class="sxs-lookup"><span data-stu-id="e9932-116">operand</span></span>|[<span data-ttu-id="e9932-117">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="e9932-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="e9932-118">Der Operand des unären Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="e9932-118">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9932-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e9932-119">Relationships</span></span>
<span data-ttu-id="e9932-120">Keine</span><span class="sxs-lookup"><span data-stu-id="e9932-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9932-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e9932-121">JSON Representation</span></span>
<span data-ttu-id="e9932-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e9932-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unaryManagementConditionExpression",
  "operator": "String",
  "operand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```




