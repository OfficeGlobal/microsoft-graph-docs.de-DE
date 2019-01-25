---
title: Ressourcentyp governanceRuleSetting
description: Stellt die Regeln, denen die rolleneinstellungen bestehen.
localization_priority: Normal
ms.openlocfilehash: bbb44760cf4b7377e5e5cc6dd312c2caee9897fa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522238"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="30beb-103">Ressourcentyp governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="30beb-103">governanceRuleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30beb-104">Stellt die Regeln, denen die rolleneinstellungen bestehen.</span><span class="sxs-lookup"><span data-stu-id="30beb-104">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="30beb-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="30beb-105">Properties</span></span>
|<span data-ttu-id="30beb-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="30beb-106">Property</span></span>      | <span data-ttu-id="30beb-107">Typ</span><span class="sxs-lookup"><span data-stu-id="30beb-107">Type</span></span>         |<span data-ttu-id="30beb-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30beb-108">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="30beb-109">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="30beb-109">ruleIdentifier</span></span>|<span data-ttu-id="30beb-110">String</span><span class="sxs-lookup"><span data-stu-id="30beb-110">String</span></span>        |<span data-ttu-id="30beb-111">Die Id der Regel.</span><span class="sxs-lookup"><span data-stu-id="30beb-111">The id of the rule.</span></span> <span data-ttu-id="30beb-112">Beispielsweise ``ExpirationRule`` und ``MfaRule``.</span><span class="sxs-lookup"><span data-stu-id="30beb-112">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="30beb-113">setting</span><span class="sxs-lookup"><span data-stu-id="30beb-113">setting</span></span>       |<span data-ttu-id="30beb-114">String</span><span class="sxs-lookup"><span data-stu-id="30beb-114">String</span></span>        |<span data-ttu-id="30beb-115">Die Einstellungen der Regel.</span><span class="sxs-lookup"><span data-stu-id="30beb-115">The settings of the rule.</span></span> <span data-ttu-id="30beb-116">Der Wert ist eine JSON-Zeichenfolge mit einer Liste von Paaren im Format Parameter_Name:Parameter_Value.</span><span class="sxs-lookup"><span data-stu-id="30beb-116">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="30beb-117">Beispiel: `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="30beb-117">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30beb-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="30beb-118">JSON representation</span></span>

<span data-ttu-id="30beb-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="30beb-119">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "governanceRuleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancerulesetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
