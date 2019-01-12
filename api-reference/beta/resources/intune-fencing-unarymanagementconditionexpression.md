---
title: Ressourcentyp unaryManagementConditionExpression
description: Ein Management Bedingungsausdruck, die mit einer Operation unärer Operator ausgewertet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 06a379a53d6d85956a54bede444714e082196ba3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949423"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="66cc5-103">Ressourcentyp unaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="66cc5-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="66cc5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="66cc5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66cc5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="66cc5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66cc5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="66cc5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66cc5-107">Ein Management Bedingungsausdruck, die mit einer Operation unärer Operator ausgewertet wird.</span><span class="sxs-lookup"><span data-stu-id="66cc5-107">A management condition expression that is evaluated using a unary operation.</span></span>

<span data-ttu-id="66cc5-108">Erbt vom [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="66cc5-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="66cc5-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="66cc5-109">Properties</span></span>
|<span data-ttu-id="66cc5-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="66cc5-110">Property</span></span>|<span data-ttu-id="66cc5-111">Typ</span><span class="sxs-lookup"><span data-stu-id="66cc5-111">Type</span></span>|<span data-ttu-id="66cc5-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66cc5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66cc5-113">operator</span><span class="sxs-lookup"><span data-stu-id="66cc5-113">operator</span></span>|[<span data-ttu-id="66cc5-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="66cc5-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="66cc5-115">Die Auswertung des Vorgangs unärer Operator verwendete Operator.</span><span class="sxs-lookup"><span data-stu-id="66cc5-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="66cc5-116">Mögliche Werte sind: `not`.</span><span class="sxs-lookup"><span data-stu-id="66cc5-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="66cc5-117">Operand</span><span class="sxs-lookup"><span data-stu-id="66cc5-117">operand</span></span>|[<span data-ttu-id="66cc5-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="66cc5-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="66cc5-119">Der Operand des Vorgangs unärer Operator.</span><span class="sxs-lookup"><span data-stu-id="66cc5-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66cc5-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="66cc5-120">Relationships</span></span>
<span data-ttu-id="66cc5-121">Keine</span><span class="sxs-lookup"><span data-stu-id="66cc5-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="66cc5-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="66cc5-122">JSON Representation</span></span>
<span data-ttu-id="66cc5-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="66cc5-123">Here is a JSON representation of the resource.</span></span>
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





