---
title: Ressourcentyp unaryManagementConditionExpression
description: Ein Management Bedingungsausdruck, die mit einer Operation unärer Operator ausgewertet wird.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f1224a869ec2ec9cae2f38273f7a68b64d3d7333
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406780"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="a35fb-103">Ressourcentyp unaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="a35fb-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="a35fb-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a35fb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a35fb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a35fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a35fb-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a35fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a35fb-107">Ein Management Bedingungsausdruck, die mit einer Operation unärer Operator ausgewertet wird.</span><span class="sxs-lookup"><span data-stu-id="a35fb-107">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="a35fb-108">Erbt vom [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="a35fb-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a35fb-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a35fb-109">Properties</span></span>
|<span data-ttu-id="a35fb-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a35fb-110">Property</span></span>|<span data-ttu-id="a35fb-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a35fb-111">Type</span></span>|<span data-ttu-id="a35fb-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a35fb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a35fb-113">operator</span><span class="sxs-lookup"><span data-stu-id="a35fb-113">operator</span></span>|[<span data-ttu-id="a35fb-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="a35fb-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="a35fb-115">Die Auswertung des Vorgangs unärer Operator verwendete Operator.</span><span class="sxs-lookup"><span data-stu-id="a35fb-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="a35fb-116">Mögliche Werte sind: `not`.</span><span class="sxs-lookup"><span data-stu-id="a35fb-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="a35fb-117">Operand</span><span class="sxs-lookup"><span data-stu-id="a35fb-117">operand</span></span>|[<span data-ttu-id="a35fb-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="a35fb-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="a35fb-119">Der Operand des Vorgangs unärer Operator.</span><span class="sxs-lookup"><span data-stu-id="a35fb-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a35fb-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a35fb-120">Relationships</span></span>
<span data-ttu-id="a35fb-121">Keine</span><span class="sxs-lookup"><span data-stu-id="a35fb-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a35fb-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a35fb-122">JSON Representation</span></span>
<span data-ttu-id="a35fb-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a35fb-123">Here is a JSON representation of the resource.</span></span>
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




