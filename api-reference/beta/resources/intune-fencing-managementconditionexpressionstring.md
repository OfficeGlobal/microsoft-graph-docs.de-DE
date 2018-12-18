---
title: Ressourcentyp managementConditionExpressionString
description: Eine Zeichenfolge Management Bedingung ist eine Zeichenfolgendarstellung eines Ausdrucks Bedingung Management.
author: tfitzmac
ms.openlocfilehash: eabcc730e86f74e2afc7c93874d47e787579c899
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361040"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="a443d-103">Ressourcentyp managementConditionExpressionString</span><span class="sxs-lookup"><span data-stu-id="a443d-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="a443d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a443d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a443d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a443d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a443d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a443d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a443d-107">Eine Zeichenfolge Management Bedingung ist eine Zeichenfolgendarstellung eines Ausdrucks Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="a443d-107">A management condition expression string is a string representation of a management condition expression.</span></span>

<span data-ttu-id="a443d-108">Erbt vom [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span><span class="sxs-lookup"><span data-stu-id="a443d-108">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a443d-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a443d-109">Properties</span></span>
|<span data-ttu-id="a443d-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a443d-110">Property</span></span>|<span data-ttu-id="a443d-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a443d-111">Type</span></span>|<span data-ttu-id="a443d-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a443d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a443d-113">Wert</span><span class="sxs-lookup"><span data-stu-id="a443d-113">value</span></span>|<span data-ttu-id="a443d-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a443d-114">String</span></span>|<span data-ttu-id="a443d-115">Die Verwaltung Condition-Anweisung Ausdruck String-Wert.</span><span class="sxs-lookup"><span data-stu-id="a443d-115">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a443d-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a443d-116">Relationships</span></span>
<span data-ttu-id="a443d-117">Keine</span><span class="sxs-lookup"><span data-stu-id="a443d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a443d-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a443d-118">JSON Representation</span></span>
<span data-ttu-id="a443d-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a443d-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementConditionExpressionString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionExpressionString",
  "value": "String"
}
```





