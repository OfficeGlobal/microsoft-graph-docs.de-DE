---
title: Ressourcentyp variableManagementConditionExpression
description: Ergibt die Bedingung Verwaltungsstatus als boolescher Ausdruck.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6a5e7efd0c8213f40d1dfb5f86d2f86c999069d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399626"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="ab30c-103">Ressourcentyp variableManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="ab30c-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="ab30c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ab30c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ab30c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ab30c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab30c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ab30c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab30c-107">Ergibt die Bedingung Verwaltungsstatus als boolescher Ausdruck.</span><span class="sxs-lookup"><span data-stu-id="ab30c-107">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="ab30c-108">Erbt vom [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="ab30c-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ab30c-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ab30c-109">Properties</span></span>
|<span data-ttu-id="ab30c-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ab30c-110">Property</span></span>|<span data-ttu-id="ab30c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="ab30c-111">Type</span></span>|<span data-ttu-id="ab30c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ab30c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab30c-113">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="ab30c-113">managementConditionId</span></span>|<span data-ttu-id="ab30c-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab30c-114">String</span></span>|<span data-ttu-id="ab30c-115">Die Bedingung Management-Id, die verwendet wird, für den Ausdruck ausgewertet werden soll.</span><span class="sxs-lookup"><span data-stu-id="ab30c-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab30c-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ab30c-116">Relationships</span></span>
<span data-ttu-id="ab30c-117">Keine</span><span class="sxs-lookup"><span data-stu-id="ab30c-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab30c-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ab30c-118">JSON Representation</span></span>
<span data-ttu-id="ab30c-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ab30c-119">Here is a JSON representation of the resource.</span></span>
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




