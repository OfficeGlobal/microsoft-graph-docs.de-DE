---
title: Ressourcentyp binaryManagementConditionExpression
description: Ein Management Bedingungsausdruck, die mit einer binären Operation ausgewertet wird.
ms.openlocfilehash: e675a5696d545ba48fc676d1716ed49c7c0b7c65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065114"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="4c43d-103">Ressourcentyp binaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="4c43d-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="4c43d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4c43d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c43d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4c43d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c43d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4c43d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c43d-107">Ein Management Bedingungsausdruck, die mit einer binären Operation ausgewertet wird.</span><span class="sxs-lookup"><span data-stu-id="4c43d-107">A management condition expression that is evaluated using a binary operation.</span></span>

<span data-ttu-id="4c43d-108">Erbt vom [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="4c43d-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4c43d-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4c43d-109">Properties</span></span>
|<span data-ttu-id="4c43d-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4c43d-110">Property</span></span>|<span data-ttu-id="4c43d-111">Typ</span><span class="sxs-lookup"><span data-stu-id="4c43d-111">Type</span></span>|<span data-ttu-id="4c43d-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c43d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c43d-113">operator</span><span class="sxs-lookup"><span data-stu-id="4c43d-113">operator</span></span>|[<span data-ttu-id="4c43d-114">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="4c43d-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="4c43d-115">Die Auswertung der binären Operation verwendete Operator.</span><span class="sxs-lookup"><span data-stu-id="4c43d-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="4c43d-116">Mögliche Werte sind: `or` und `and`.</span><span class="sxs-lookup"><span data-stu-id="4c43d-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="4c43d-117">firstOperand</span><span class="sxs-lookup"><span data-stu-id="4c43d-117">firstOperand</span></span>|[<span data-ttu-id="4c43d-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="4c43d-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="4c43d-119">Dem ersten Operanden der binären Operation.</span><span class="sxs-lookup"><span data-stu-id="4c43d-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="4c43d-120">secondOperand</span><span class="sxs-lookup"><span data-stu-id="4c43d-120">secondOperand</span></span>|[<span data-ttu-id="4c43d-121">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="4c43d-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="4c43d-122">Der zweite Operand des binären Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="4c43d-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c43d-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4c43d-123">Relationships</span></span>
<span data-ttu-id="4c43d-124">Keine</span><span class="sxs-lookup"><span data-stu-id="4c43d-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4c43d-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4c43d-125">JSON Representation</span></span>
<span data-ttu-id="4c43d-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4c43d-126">Here is a JSON representation of the resource.</span></span>
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





