---
title: Ressourcentyp binaryManagementConditionExpression
description: Ein Management Bedingungsausdruck, die mit einer binären Operation ausgewertet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b15938d0bb29fdfdad8abb1b37b02ad1e6468cf9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978536"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="fa919-103">Ressourcentyp binaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="fa919-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="fa919-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fa919-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa919-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa919-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa919-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fa919-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa919-107">Ein Management Bedingungsausdruck, die mit einer binären Operation ausgewertet wird.</span><span class="sxs-lookup"><span data-stu-id="fa919-107">A management condition expression that is evaluated using a binary operation.</span></span>

<span data-ttu-id="fa919-108">Erbt vom [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="fa919-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fa919-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fa919-109">Properties</span></span>
|<span data-ttu-id="fa919-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa919-110">Property</span></span>|<span data-ttu-id="fa919-111">Typ</span><span class="sxs-lookup"><span data-stu-id="fa919-111">Type</span></span>|<span data-ttu-id="fa919-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa919-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa919-113">operator</span><span class="sxs-lookup"><span data-stu-id="fa919-113">operator</span></span>|[<span data-ttu-id="fa919-114">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="fa919-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="fa919-115">Die Auswertung der binären Operation verwendete Operator.</span><span class="sxs-lookup"><span data-stu-id="fa919-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="fa919-116">Mögliche Werte sind: `or` und `and`.</span><span class="sxs-lookup"><span data-stu-id="fa919-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="fa919-117">firstOperand</span><span class="sxs-lookup"><span data-stu-id="fa919-117">firstOperand</span></span>|[<span data-ttu-id="fa919-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="fa919-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="fa919-119">Dem ersten Operanden der binären Operation.</span><span class="sxs-lookup"><span data-stu-id="fa919-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="fa919-120">secondOperand</span><span class="sxs-lookup"><span data-stu-id="fa919-120">secondOperand</span></span>|[<span data-ttu-id="fa919-121">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="fa919-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="fa919-122">Der zweite Operand des binären Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="fa919-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa919-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fa919-123">Relationships</span></span>
<span data-ttu-id="fa919-124">Keine</span><span class="sxs-lookup"><span data-stu-id="fa919-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fa919-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fa919-125">JSON Representation</span></span>
<span data-ttu-id="fa919-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fa919-126">Here is a JSON representation of the resource.</span></span>
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





