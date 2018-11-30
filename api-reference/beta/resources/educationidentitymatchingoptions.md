---
title: Ressourcentyp educationIdentityMatchingOptions
description: Stellt eine Zuordnung zwischen einem Source-Eigenschaft und einer Target-Eigenschaft für den Abgleich von Benutzerkonten bereit. Die Source-Eigenschaft sollte in den Quelldaten vorhanden sein. Target-Eigenschaft muss eine gültige Eigenschaft in Azure Active Directory (AD Azure) sein.
ms.openlocfilehash: 2cabb255648f4089d437912a97bb7d29ff286779
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063548"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="0635c-105">Ressourcentyp educationIdentityMatchingOptions</span><span class="sxs-lookup"><span data-stu-id="0635c-105">educationIdentityMatchingOptions resource type</span></span>

> <span data-ttu-id="0635c-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0635c-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0635c-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0635c-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0635c-108">Stellt eine Zuordnung zwischen einem Source-Eigenschaft und einer Target-Eigenschaft für den Abgleich von Benutzerkonten bereit.</span><span class="sxs-lookup"><span data-stu-id="0635c-108">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="0635c-109">Die Source-Eigenschaft sollte in den Quelldaten vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="0635c-109">The source property should exist in the source data.</span></span> <span data-ttu-id="0635c-110">Target-Eigenschaft muss eine gültige Eigenschaft in Azure Active Directory (AD Azure) sein.</span><span class="sxs-lookup"><span data-stu-id="0635c-110">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="0635c-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0635c-111">Properties</span></span>

| <span data-ttu-id="0635c-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0635c-112">Property</span></span> | <span data-ttu-id="0635c-113">Typ</span><span class="sxs-lookup"><span data-stu-id="0635c-113">Type</span></span> | <span data-ttu-id="0635c-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0635c-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="0635c-115">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="0635c-115">**appliesTo**</span></span> | <span data-ttu-id="0635c-116">string</span><span class="sxs-lookup"><span data-stu-id="0635c-116">string</span></span> |  <span data-ttu-id="0635c-117">Der Benutzer Rollentyp die Lizenz zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="0635c-117">The user role type to assign to the license.</span></span> <span data-ttu-id="0635c-118">Mögliche Werte sind: `student` und `teacher`.</span><span class="sxs-lookup"><span data-stu-id="0635c-118">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="0635c-119">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="0635c-119">**sourcePropertyName**</span></span> | <span data-ttu-id="0635c-120">string</span><span class="sxs-lookup"><span data-stu-id="0635c-120">string</span></span> |  <span data-ttu-id="0635c-121">Der Name der Source-Eigenschaft, die ein Feldname in den Quelldaten sein sollte.</span><span class="sxs-lookup"><span data-stu-id="0635c-121">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="0635c-122">Diese Eigenschaft wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="0635c-122">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="0635c-123">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="0635c-123">**targetPropertyName**</span></span> | <span data-ttu-id="0635c-124">string</span><span class="sxs-lookup"><span data-stu-id="0635c-124">string</span></span> |  <span data-ttu-id="0635c-125">Der Name der Zieleigenschaft, die eine gültige Eigenschaft in Azure AD sein sollte.</span><span class="sxs-lookup"><span data-stu-id="0635c-125">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="0635c-126">Diese Eigenschaft wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="0635c-126">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="0635c-127">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="0635c-127">**targetDomain**</span></span> | <span data-ttu-id="0635c-128">string</span><span class="sxs-lookup"><span data-stu-id="0635c-128">string</span></span> |  <span data-ttu-id="0635c-129">Die Domäne, mit der Source-Eigenschaft im Ziel übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="0635c-129">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="0635c-130">Wenn als null angegeben wird, wird die Source-Eigenschaft verwendet werden, der mit der Zieleigenschaft entspricht.</span><span class="sxs-lookup"><span data-stu-id="0635c-130">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="0635c-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0635c-131">JSON representation</span></span>
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
