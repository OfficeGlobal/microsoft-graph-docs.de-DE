---
title: Ressourcentyp variableManagementConditionExpression
description: Ergibt die Bedingung Verwaltungsstatus als boolescher Ausdruck.
ms.openlocfilehash: 220cb54680755461edb9dab6edf076f8ae0c6a68
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062476"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="87d23-103">Ressourcentyp variableManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="87d23-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="87d23-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="87d23-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87d23-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="87d23-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87d23-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="87d23-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87d23-107">Ergibt die Bedingung Verwaltungsstatus als boolescher Ausdruck.</span><span class="sxs-lookup"><span data-stu-id="87d23-107">Evaluates the management condition state as a Boolean expression.</span></span>

<span data-ttu-id="87d23-108">Erbt vom [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="87d23-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="87d23-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="87d23-109">Properties</span></span>
|<span data-ttu-id="87d23-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="87d23-110">Property</span></span>|<span data-ttu-id="87d23-111">Typ</span><span class="sxs-lookup"><span data-stu-id="87d23-111">Type</span></span>|<span data-ttu-id="87d23-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87d23-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87d23-113">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="87d23-113">managementConditionId</span></span>|<span data-ttu-id="87d23-114">String</span><span class="sxs-lookup"><span data-stu-id="87d23-114">String</span></span>|<span data-ttu-id="87d23-115">Die Bedingung Management-Id, die verwendet wird, für den Ausdruck ausgewertet werden soll.</span><span class="sxs-lookup"><span data-stu-id="87d23-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87d23-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="87d23-116">Relationships</span></span>
<span data-ttu-id="87d23-117">Keine</span><span class="sxs-lookup"><span data-stu-id="87d23-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="87d23-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="87d23-118">JSON Representation</span></span>
<span data-ttu-id="87d23-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="87d23-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.variableManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.variableManagementConditionExpression",
  "managementConditionId": "String"
}
```





