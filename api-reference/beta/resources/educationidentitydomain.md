---
title: Ressourcentyp educationIdentityDomain
description: 'Stellt die Zuordnung zwischen einer Education Benutzertyp und der Domäne, der das Konto des Benutzers gehört. Die Domänenressource ist Teil der Identity-Konfiguration erstellen. '
localization_priority: Normal
ms.openlocfilehash: 5675499aca010f90deeb517210065ac4802d66b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807749"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="46471-104">Ressourcentyp educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="46471-104">educationIdentityDomain resource type</span></span>

> <span data-ttu-id="46471-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="46471-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46471-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="46471-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="46471-107">Stellt die Zuordnung zwischen einer Education Benutzertyp und der Domäne, der das Konto des Benutzers gehört.</span><span class="sxs-lookup"><span data-stu-id="46471-107">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="46471-108">Die Domänenressource ist Teil der [Identität Erstellung Konfiguration](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46471-108">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="46471-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="46471-109">Properties</span></span>

| <span data-ttu-id="46471-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="46471-110">Property</span></span> | <span data-ttu-id="46471-111">Typ</span><span class="sxs-lookup"><span data-stu-id="46471-111">Type</span></span> | <span data-ttu-id="46471-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46471-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="46471-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="46471-113">**appliesTo**</span></span> | <span data-ttu-id="46471-114">string</span><span class="sxs-lookup"><span data-stu-id="46471-114">string</span></span> |  <span data-ttu-id="46471-115">Der Benutzer Rollentyp Lizenz zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="46471-115">The user role type to assign to license.</span></span> <span data-ttu-id="46471-116">Mögliche Werte sind: `student` und `teacher`.</span><span class="sxs-lookup"><span data-stu-id="46471-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="46471-117">**name**</span><span class="sxs-lookup"><span data-stu-id="46471-117">**name**</span></span> | <span data-ttu-id="46471-118">string</span><span class="sxs-lookup"><span data-stu-id="46471-118">string</span></span> |  <span data-ttu-id="46471-119">Stellt die Domäne für das Benutzerkonto ein.</span><span class="sxs-lookup"><span data-stu-id="46471-119">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="46471-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="46471-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "name": "String"
}
```
