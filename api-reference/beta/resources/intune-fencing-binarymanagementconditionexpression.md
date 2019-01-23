---
title: Ressourcentyp binaryManagementConditionExpression
description: Ein Management Bedingungsausdruck, die mit einer binären Operation ausgewertet wird.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 722387492e6167c3bd74d306fa03e4835bc12dbe
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402727"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="5fab9-103">Ressourcentyp binaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="5fab9-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="5fab9-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="5fab9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5fab9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5fab9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5fab9-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5fab9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fab9-107">Ein Management Bedingungsausdruck, die mit einer binären Operation ausgewertet wird.</span><span class="sxs-lookup"><span data-stu-id="5fab9-107">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="5fab9-108">Erbt vom [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="5fab9-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5fab9-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5fab9-109">Properties</span></span>
|<span data-ttu-id="5fab9-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5fab9-110">Property</span></span>|<span data-ttu-id="5fab9-111">Typ</span><span class="sxs-lookup"><span data-stu-id="5fab9-111">Type</span></span>|<span data-ttu-id="5fab9-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5fab9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fab9-113">operator</span><span class="sxs-lookup"><span data-stu-id="5fab9-113">operator</span></span>|[<span data-ttu-id="5fab9-114">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="5fab9-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="5fab9-115">Die Auswertung der binären Operation verwendete Operator.</span><span class="sxs-lookup"><span data-stu-id="5fab9-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="5fab9-116">Mögliche Werte sind: `or` und `and`.</span><span class="sxs-lookup"><span data-stu-id="5fab9-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="5fab9-117">firstOperand</span><span class="sxs-lookup"><span data-stu-id="5fab9-117">firstOperand</span></span>|[<span data-ttu-id="5fab9-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="5fab9-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="5fab9-119">Dem ersten Operanden der binären Operation.</span><span class="sxs-lookup"><span data-stu-id="5fab9-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="5fab9-120">secondOperand</span><span class="sxs-lookup"><span data-stu-id="5fab9-120">secondOperand</span></span>|[<span data-ttu-id="5fab9-121">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="5fab9-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="5fab9-122">Der zweite Operand des binären Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="5fab9-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fab9-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5fab9-123">Relationships</span></span>
<span data-ttu-id="5fab9-124">Keine</span><span class="sxs-lookup"><span data-stu-id="5fab9-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5fab9-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5fab9-125">JSON Representation</span></span>
<span data-ttu-id="5fab9-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5fab9-126">Here is a JSON representation of the resource.</span></span>
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




