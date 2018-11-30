---
title: Ressourcentyp managementConditionExpressionString
description: Eine Zeichenfolge Management Bedingung ist eine Zeichenfolgendarstellung eines Ausdrucks Bedingung Management.
ms.openlocfilehash: 456df27900aa10ead7e2bc090e5e06e0bcd7754f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065115"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="7cd96-103">Ressourcentyp managementConditionExpressionString</span><span class="sxs-lookup"><span data-stu-id="7cd96-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="7cd96-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7cd96-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7cd96-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7cd96-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7cd96-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7cd96-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7cd96-107">Eine Zeichenfolge Management Bedingung ist eine Zeichenfolgendarstellung eines Ausdrucks Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="7cd96-107">A management condition expression string is a string representation of a management condition expression.</span></span>

<span data-ttu-id="7cd96-108">Erbt vom [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span><span class="sxs-lookup"><span data-stu-id="7cd96-108">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7cd96-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7cd96-109">Properties</span></span>
|<span data-ttu-id="7cd96-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7cd96-110">Property</span></span>|<span data-ttu-id="7cd96-111">Typ</span><span class="sxs-lookup"><span data-stu-id="7cd96-111">Type</span></span>|<span data-ttu-id="7cd96-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7cd96-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cd96-113">Wert</span><span class="sxs-lookup"><span data-stu-id="7cd96-113">value</span></span>|<span data-ttu-id="7cd96-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7cd96-114">String</span></span>|<span data-ttu-id="7cd96-115">Die Verwaltung Condition-Anweisung Ausdruck String-Wert.</span><span class="sxs-lookup"><span data-stu-id="7cd96-115">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7cd96-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7cd96-116">Relationships</span></span>
<span data-ttu-id="7cd96-117">Keine</span><span class="sxs-lookup"><span data-stu-id="7cd96-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7cd96-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7cd96-118">JSON Representation</span></span>
<span data-ttu-id="7cd96-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7cd96-119">Here is a JSON representation of the resource.</span></span>
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





