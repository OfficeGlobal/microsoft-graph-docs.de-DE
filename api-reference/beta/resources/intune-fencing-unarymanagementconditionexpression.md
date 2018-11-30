---
title: Ressourcentyp unaryManagementConditionExpression
description: Ein Management Bedingungsausdruck, die mit einer Operation unärer Operator ausgewertet wird.
ms.openlocfilehash: 958c180e52a268f849eca1fe0d2a2b75ff81333b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062191"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="494aa-103">Ressourcentyp unaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="494aa-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="494aa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="494aa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="494aa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="494aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="494aa-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="494aa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="494aa-107">Ein Management Bedingungsausdruck, die mit einer Operation unärer Operator ausgewertet wird.</span><span class="sxs-lookup"><span data-stu-id="494aa-107">A management condition expression that is evaluated using a unary operation.</span></span>

<span data-ttu-id="494aa-108">Erbt vom [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="494aa-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="494aa-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="494aa-109">Properties</span></span>
|<span data-ttu-id="494aa-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="494aa-110">Property</span></span>|<span data-ttu-id="494aa-111">Typ</span><span class="sxs-lookup"><span data-stu-id="494aa-111">Type</span></span>|<span data-ttu-id="494aa-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="494aa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="494aa-113">operator</span><span class="sxs-lookup"><span data-stu-id="494aa-113">operator</span></span>|[<span data-ttu-id="494aa-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="494aa-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="494aa-115">Die Auswertung des Vorgangs unärer Operator verwendete Operator.</span><span class="sxs-lookup"><span data-stu-id="494aa-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="494aa-116">Mögliche Werte sind: `not`.</span><span class="sxs-lookup"><span data-stu-id="494aa-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="494aa-117">Operand</span><span class="sxs-lookup"><span data-stu-id="494aa-117">operand</span></span>|[<span data-ttu-id="494aa-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="494aa-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="494aa-119">Der Operand des Vorgangs unärer Operator.</span><span class="sxs-lookup"><span data-stu-id="494aa-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="494aa-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="494aa-120">Relationships</span></span>
<span data-ttu-id="494aa-121">Keine</span><span class="sxs-lookup"><span data-stu-id="494aa-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="494aa-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="494aa-122">JSON Representation</span></span>
<span data-ttu-id="494aa-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="494aa-123">Here is a JSON representation of the resource.</span></span>
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





