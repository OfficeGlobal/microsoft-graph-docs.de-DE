---
title: variableManagementConditionExpression-Ressourcentyp
description: Wertet den Status der Verwaltungsbedingung als booleschen Ausdruck aus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fab070cc9d2c51fbe1dc4b33c82fb823a849b7cc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168229"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="4cc0d-103">variableManagementConditionExpression-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4cc0d-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="4cc0d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4cc0d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cc0d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4cc0d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cc0d-106">Wertet den Status der Verwaltungsbedingung als booleschen Ausdruck aus.</span><span class="sxs-lookup"><span data-stu-id="4cc0d-106">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="4cc0d-107">Erbt von [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="4cc0d-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4cc0d-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4cc0d-108">Properties</span></span>
|<span data-ttu-id="4cc0d-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4cc0d-109">Property</span></span>|<span data-ttu-id="4cc0d-110">Typ</span><span class="sxs-lookup"><span data-stu-id="4cc0d-110">Type</span></span>|<span data-ttu-id="4cc0d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4cc0d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cc0d-112">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="4cc0d-112">managementConditionId</span></span>|<span data-ttu-id="4cc0d-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4cc0d-113">String</span></span>|<span data-ttu-id="4cc0d-114">Die Verwaltungs Bedingungs-ID, die zum Auswerten des Ausdrucks verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="4cc0d-114">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cc0d-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4cc0d-115">Relationships</span></span>
<span data-ttu-id="4cc0d-116">Keine</span><span class="sxs-lookup"><span data-stu-id="4cc0d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4cc0d-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4cc0d-117">JSON Representation</span></span>
<span data-ttu-id="4cc0d-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4cc0d-118">Here is a JSON representation of the resource.</span></span>
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




