---
title: Ressourcentyp governanceRuleSetting
description: Stellt die Regeln, denen die rolleneinstellungen bestehen.
ms.openlocfilehash: 486b5163c59772c971cfc1d61a98817b7f0c16f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062344"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="c54c4-103">Ressourcentyp governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="c54c4-103">governanceRuleSetting resource type</span></span>

> <span data-ttu-id="c54c4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c54c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c54c4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c54c4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c54c4-106">Stellt die Regeln, denen die rolleneinstellungen bestehen.</span><span class="sxs-lookup"><span data-stu-id="c54c4-106">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="c54c4-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c54c4-107">Properties</span></span>
|<span data-ttu-id="c54c4-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c54c4-108">Property</span></span>      | <span data-ttu-id="c54c4-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c54c4-109">Type</span></span>         |<span data-ttu-id="c54c4-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c54c4-110">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="c54c4-111">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="c54c4-111">ruleIdentifier</span></span>|<span data-ttu-id="c54c4-112">String</span><span class="sxs-lookup"><span data-stu-id="c54c4-112">String</span></span>        |<span data-ttu-id="c54c4-113">Die Id der Regel.</span><span class="sxs-lookup"><span data-stu-id="c54c4-113">The id of the rule.</span></span> <span data-ttu-id="c54c4-114">Beispielsweise ``ExpirationRule`` und ``MfaRule``.</span><span class="sxs-lookup"><span data-stu-id="c54c4-114">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="c54c4-115">setting</span><span class="sxs-lookup"><span data-stu-id="c54c4-115">setting</span></span>       |<span data-ttu-id="c54c4-116">String</span><span class="sxs-lookup"><span data-stu-id="c54c4-116">String</span></span>        |<span data-ttu-id="c54c4-117">Die Einstellungen der Regel.</span><span class="sxs-lookup"><span data-stu-id="c54c4-117">The settings of the rule.</span></span> <span data-ttu-id="c54c4-118">Der Wert ist eine JSON-Zeichenfolge mit einer Liste von Paaren im Format Parameter_Name:Parameter_Value.</span><span class="sxs-lookup"><span data-stu-id="c54c4-118">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="c54c4-119">Beispielsweise gibt `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="c54c4-119">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c54c4-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c54c4-120">JSON representation</span></span>

<span data-ttu-id="c54c4-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c54c4-121">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRuleSetting"
}-->


```json
{
  "ruleIdentifier": "String",
  "setting": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRuleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->