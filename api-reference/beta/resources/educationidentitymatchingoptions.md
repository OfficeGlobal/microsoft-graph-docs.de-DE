---
title: Ressourcentyp educationIdentityMatchingOptions
description: Stellt eine Zuordnung zwischen einem Source-Eigenschaft und einer Target-Eigenschaft für den Abgleich von Benutzerkonten bereit. Die Source-Eigenschaft sollte in den Quelldaten vorhanden sein. Target-Eigenschaft muss eine gültige Eigenschaft in Azure Active Directory (AD Azure) sein.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 723a74cff1d5a660272d3456e9f54de8a54e21bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513704"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="32f4b-105">Ressourcentyp educationIdentityMatchingOptions</span><span class="sxs-lookup"><span data-stu-id="32f4b-105">educationIdentityMatchingOptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32f4b-106">Stellt eine Zuordnung zwischen einem Source-Eigenschaft und einer Target-Eigenschaft für den Abgleich von Benutzerkonten bereit.</span><span class="sxs-lookup"><span data-stu-id="32f4b-106">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="32f4b-107">Die Source-Eigenschaft sollte in den Quelldaten vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="32f4b-107">The source property should exist in the source data.</span></span> <span data-ttu-id="32f4b-108">Target-Eigenschaft muss eine gültige Eigenschaft in Azure Active Directory (AD Azure) sein.</span><span class="sxs-lookup"><span data-stu-id="32f4b-108">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="32f4b-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="32f4b-109">Properties</span></span>

| <span data-ttu-id="32f4b-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="32f4b-110">Property</span></span> | <span data-ttu-id="32f4b-111">Typ</span><span class="sxs-lookup"><span data-stu-id="32f4b-111">Type</span></span> | <span data-ttu-id="32f4b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32f4b-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="32f4b-113">appliesTo</span><span class="sxs-lookup"><span data-stu-id="32f4b-113">**appliesTo**</span></span> | <span data-ttu-id="32f4b-114">string</span><span class="sxs-lookup"><span data-stu-id="32f4b-114">string</span></span> |  <span data-ttu-id="32f4b-115">Der Benutzer Rollentyp die Lizenz zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="32f4b-115">The user role type to assign to the license.</span></span> <span data-ttu-id="32f4b-116">Mögliche Werte sind: `student` und `teacher`.</span><span class="sxs-lookup"><span data-stu-id="32f4b-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="32f4b-117">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="32f4b-117">**sourcePropertyName**</span></span> | <span data-ttu-id="32f4b-118">string</span><span class="sxs-lookup"><span data-stu-id="32f4b-118">string</span></span> |  <span data-ttu-id="32f4b-119">Der Name der Source-Eigenschaft, die ein Feldname in den Quelldaten sein sollte.</span><span class="sxs-lookup"><span data-stu-id="32f4b-119">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="32f4b-120">Diese Eigenschaft wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="32f4b-120">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="32f4b-121">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="32f4b-121">**targetPropertyName**</span></span> | <span data-ttu-id="32f4b-122">string</span><span class="sxs-lookup"><span data-stu-id="32f4b-122">string</span></span> |  <span data-ttu-id="32f4b-123">Der Name der Zieleigenschaft, die eine gültige Eigenschaft in Azure AD sein sollte.</span><span class="sxs-lookup"><span data-stu-id="32f4b-123">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="32f4b-124">Diese Eigenschaft wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="32f4b-124">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="32f4b-125">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="32f4b-125">**targetDomain**</span></span> | <span data-ttu-id="32f4b-126">string</span><span class="sxs-lookup"><span data-stu-id="32f4b-126">string</span></span> |  <span data-ttu-id="32f4b-127">Die Domäne, mit der Source-Eigenschaft im Ziel übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="32f4b-127">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="32f4b-128">Wenn als null angegeben wird, wird die Source-Eigenschaft verwendet werden, der mit der Zieleigenschaft entspricht.</span><span class="sxs-lookup"><span data-stu-id="32f4b-128">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="32f4b-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="32f4b-129">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitymatchingoptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
