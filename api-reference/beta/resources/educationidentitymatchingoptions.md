---
title: Ressourcentyp educationIdentityMatchingOptions
description: Stellt eine Zuordnung zwischen einem Source-Eigenschaft und einer Target-Eigenschaft für den Abgleich von Benutzerkonten bereit. Die Source-Eigenschaft sollte in den Quelldaten vorhanden sein. Target-Eigenschaft muss eine gültige Eigenschaft in Azure Active Directory (AD Azure) sein.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 80e9222f8f0c03294a947f403b33cc4f2cd2ef0f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876279"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="b3227-105">Ressourcentyp educationIdentityMatchingOptions</span><span class="sxs-lookup"><span data-stu-id="b3227-105">educationIdentityMatchingOptions resource type</span></span>

> <span data-ttu-id="b3227-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b3227-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3227-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b3227-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b3227-108">Stellt eine Zuordnung zwischen einem Source-Eigenschaft und einer Target-Eigenschaft für den Abgleich von Benutzerkonten bereit.</span><span class="sxs-lookup"><span data-stu-id="b3227-108">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="b3227-109">Die Source-Eigenschaft sollte in den Quelldaten vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="b3227-109">The source property should exist in the source data.</span></span> <span data-ttu-id="b3227-110">Target-Eigenschaft muss eine gültige Eigenschaft in Azure Active Directory (AD Azure) sein.</span><span class="sxs-lookup"><span data-stu-id="b3227-110">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="b3227-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b3227-111">Properties</span></span>

| <span data-ttu-id="b3227-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b3227-112">Property</span></span> | <span data-ttu-id="b3227-113">Typ</span><span class="sxs-lookup"><span data-stu-id="b3227-113">Type</span></span> | <span data-ttu-id="b3227-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3227-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b3227-115">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="b3227-115">**appliesTo**</span></span> | <span data-ttu-id="b3227-116">string</span><span class="sxs-lookup"><span data-stu-id="b3227-116">string</span></span> |  <span data-ttu-id="b3227-117">Der Benutzer Rollentyp die Lizenz zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="b3227-117">The user role type to assign to the license.</span></span> <span data-ttu-id="b3227-118">Mögliche Werte sind: `student` und `teacher`.</span><span class="sxs-lookup"><span data-stu-id="b3227-118">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="b3227-119">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="b3227-119">**sourcePropertyName**</span></span> | <span data-ttu-id="b3227-120">string</span><span class="sxs-lookup"><span data-stu-id="b3227-120">string</span></span> |  <span data-ttu-id="b3227-121">Der Name der Source-Eigenschaft, die ein Feldname in den Quelldaten sein sollte.</span><span class="sxs-lookup"><span data-stu-id="b3227-121">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="b3227-122">Diese Eigenschaft wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="b3227-122">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="b3227-123">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="b3227-123">**targetPropertyName**</span></span> | <span data-ttu-id="b3227-124">string</span><span class="sxs-lookup"><span data-stu-id="b3227-124">string</span></span> |  <span data-ttu-id="b3227-125">Der Name der Zieleigenschaft, die eine gültige Eigenschaft in Azure AD sein sollte.</span><span class="sxs-lookup"><span data-stu-id="b3227-125">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="b3227-126">Diese Eigenschaft wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="b3227-126">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="b3227-127">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="b3227-127">**targetDomain**</span></span> | <span data-ttu-id="b3227-128">string</span><span class="sxs-lookup"><span data-stu-id="b3227-128">string</span></span> |  <span data-ttu-id="b3227-129">Die Domäne, mit der Source-Eigenschaft im Ziel übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="b3227-129">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="b3227-130">Wenn als null angegeben wird, wird die Source-Eigenschaft verwendet werden, der mit der Zieleigenschaft entspricht.</span><span class="sxs-lookup"><span data-stu-id="b3227-130">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="b3227-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b3227-131">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
