---
title: binaryManagementConditionExpression-Ressourcentyp
description: Ein Ausdruck der Verwaltungsbedingung, der mit einem binären Vorgang ausgewertet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d70306923b86f6d42942c5ce6b78ff31819d47d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150484"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="d09a8-103">binaryManagementConditionExpression-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d09a8-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="d09a8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d09a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d09a8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d09a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d09a8-106">Ein Ausdruck der Verwaltungsbedingung, der mit einem binären Vorgang ausgewertet wird.</span><span class="sxs-lookup"><span data-stu-id="d09a8-106">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="d09a8-107">Erbt von [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="d09a8-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d09a8-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d09a8-108">Properties</span></span>
|<span data-ttu-id="d09a8-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d09a8-109">Property</span></span>|<span data-ttu-id="d09a8-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d09a8-110">Type</span></span>|<span data-ttu-id="d09a8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d09a8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d09a8-112">operator</span><span class="sxs-lookup"><span data-stu-id="d09a8-112">operator</span></span>|[<span data-ttu-id="d09a8-113">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="d09a8-113">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="d09a8-114">Der Operator, der bei der Auswertung des Binär Vorgangs verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="d09a8-114">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="d09a8-115">Mögliche Werte sind: `or` und `and`.</span><span class="sxs-lookup"><span data-stu-id="d09a8-115">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="d09a8-116">firstOperand</span><span class="sxs-lookup"><span data-stu-id="d09a8-116">firstOperand</span></span>|[<span data-ttu-id="d09a8-117">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="d09a8-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="d09a8-118">Der erste Operand des binären Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="d09a8-118">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="d09a8-119">secondOperand</span><span class="sxs-lookup"><span data-stu-id="d09a8-119">secondOperand</span></span>|[<span data-ttu-id="d09a8-120">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="d09a8-120">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="d09a8-121">Der zweite Operand des binären Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="d09a8-121">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d09a8-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d09a8-122">Relationships</span></span>
<span data-ttu-id="d09a8-123">Keine</span><span class="sxs-lookup"><span data-stu-id="d09a8-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d09a8-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d09a8-124">JSON Representation</span></span>
<span data-ttu-id="d09a8-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d09a8-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.binaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.binaryManagementConditionExpression",
  "operator": "String",
  "firstOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  },
  "secondOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```




