---
title: Ressourcentyp unaryManagementConditionExpression
description: Ein Management Bedingungsausdruck, die mit einer Operation unärer Operator ausgewertet wird.
author: tfitzmac
ms.openlocfilehash: 43711e68d88bdf0854e8501377fbf3e30b25b3ec
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344345"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="e4f8c-103">Ressourcentyp unaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="e4f8c-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="e4f8c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e4f8c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4f8c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e4f8c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4f8c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e4f8c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4f8c-107">Ein Management Bedingungsausdruck, die mit einer Operation unärer Operator ausgewertet wird.</span><span class="sxs-lookup"><span data-stu-id="e4f8c-107">A management condition expression that is evaluated using a unary operation.</span></span>

<span data-ttu-id="e4f8c-108">Erbt vom [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="e4f8c-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e4f8c-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e4f8c-109">Properties</span></span>
|<span data-ttu-id="e4f8c-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e4f8c-110">Property</span></span>|<span data-ttu-id="e4f8c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="e4f8c-111">Type</span></span>|<span data-ttu-id="e4f8c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4f8c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4f8c-113">operator</span><span class="sxs-lookup"><span data-stu-id="e4f8c-113">operator</span></span>|[<span data-ttu-id="e4f8c-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="e4f8c-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="e4f8c-115">Die Auswertung des Vorgangs unärer Operator verwendete Operator.</span><span class="sxs-lookup"><span data-stu-id="e4f8c-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="e4f8c-116">Mögliche Werte sind: `not`.</span><span class="sxs-lookup"><span data-stu-id="e4f8c-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="e4f8c-117">Operand</span><span class="sxs-lookup"><span data-stu-id="e4f8c-117">operand</span></span>|[<span data-ttu-id="e4f8c-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="e4f8c-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="e4f8c-119">Der Operand des Vorgangs unärer Operator.</span><span class="sxs-lookup"><span data-stu-id="e4f8c-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4f8c-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e4f8c-120">Relationships</span></span>
<span data-ttu-id="e4f8c-121">Keine</span><span class="sxs-lookup"><span data-stu-id="e4f8c-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e4f8c-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e4f8c-122">JSON Representation</span></span>
<span data-ttu-id="e4f8c-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e4f8c-123">Here is a JSON representation of the resource.</span></span>
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





