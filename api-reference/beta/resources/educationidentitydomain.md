---
title: Ressourcentyp educationIdentityDomain
description: 'Stellt die Zuordnung zwischen einer Education Benutzertyp und der Domäne, der das Konto des Benutzers gehört. Die Domänenressource ist Teil der Identity-Konfiguration erstellen. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 0c6004d18897b8f8284c06a3b09830072148df87
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528179"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="69fa6-104">Ressourcentyp educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="69fa6-104">educationIdentityDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69fa6-105">Stellt die Zuordnung zwischen einer Education Benutzertyp und der Domäne, der das Konto des Benutzers gehört.</span><span class="sxs-lookup"><span data-stu-id="69fa6-105">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="69fa6-106">Die Domänenressource ist Teil der [Identität Erstellung Konfiguration](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69fa6-106">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="69fa6-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="69fa6-107">Properties</span></span>

| <span data-ttu-id="69fa6-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="69fa6-108">Property</span></span> | <span data-ttu-id="69fa6-109">Typ</span><span class="sxs-lookup"><span data-stu-id="69fa6-109">Type</span></span> | <span data-ttu-id="69fa6-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69fa6-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="69fa6-111">appliesTo</span><span class="sxs-lookup"><span data-stu-id="69fa6-111">**appliesTo**</span></span> | <span data-ttu-id="69fa6-112">string</span><span class="sxs-lookup"><span data-stu-id="69fa6-112">string</span></span> |  <span data-ttu-id="69fa6-113">Der Benutzer Rollentyp Lizenz zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="69fa6-113">The user role type to assign to license.</span></span> <span data-ttu-id="69fa6-114">Mögliche Werte sind: `student` und `teacher`.</span><span class="sxs-lookup"><span data-stu-id="69fa6-114">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="69fa6-115">**name**</span><span class="sxs-lookup"><span data-stu-id="69fa6-115">**name**</span></span> | <span data-ttu-id="69fa6-116">string</span><span class="sxs-lookup"><span data-stu-id="69fa6-116">string</span></span> |  <span data-ttu-id="69fa6-117">Stellt die Domäne für das Benutzerkonto ein.</span><span class="sxs-lookup"><span data-stu-id="69fa6-117">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="69fa6-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="69fa6-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "name": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitydomain.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
