---
title: managementConditionExpressionString-Ressourcentyp
description: Eine Ausdruckszeichenfolge für die Verwaltungsbedingung ist eine Zeichenfolgendarstellung eines Ausdrucks der Verwaltungsbedingung.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc4552ab6cc97676ced32ae7e7f5649262c4f4f7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151009"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="58b83-103">managementConditionExpressionString-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="58b83-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="58b83-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="58b83-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58b83-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="58b83-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58b83-106">Eine Ausdruckszeichenfolge für die Verwaltungsbedingung ist eine Zeichenfolgendarstellung eines Ausdrucks der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="58b83-106">A management condition expression string is a string representation of a management condition expression.</span></span>


<span data-ttu-id="58b83-107">Erbt von [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span><span class="sxs-lookup"><span data-stu-id="58b83-107">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="58b83-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="58b83-108">Properties</span></span>
|<span data-ttu-id="58b83-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="58b83-109">Property</span></span>|<span data-ttu-id="58b83-110">Typ</span><span class="sxs-lookup"><span data-stu-id="58b83-110">Type</span></span>|<span data-ttu-id="58b83-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58b83-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58b83-112">Wert</span><span class="sxs-lookup"><span data-stu-id="58b83-112">value</span></span>|<span data-ttu-id="58b83-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58b83-113">String</span></span>|<span data-ttu-id="58b83-114">Der Ausdruck String-Wert der Verwaltungs Bedingungsanweisung.</span><span class="sxs-lookup"><span data-stu-id="58b83-114">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58b83-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="58b83-115">Relationships</span></span>
<span data-ttu-id="58b83-116">Keine</span><span class="sxs-lookup"><span data-stu-id="58b83-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58b83-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="58b83-117">JSON Representation</span></span>
<span data-ttu-id="58b83-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="58b83-118">Here is a JSON representation of the resource.</span></span>
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




