---
title: Ressourcentyp educationIdentityDomain
description: 'Stellt die Zuordnung zwischen einer Education Benutzertyp und der Domäne, der das Konto des Benutzers gehört. Die Domänenressource ist Teil der Identity-Konfiguration erstellen. '
ms.openlocfilehash: 8298e1eb38ae70f982719ee3a7d6588cd181bdd8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063349"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="0db18-104">Ressourcentyp educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="0db18-104">educationIdentityDomain resource type</span></span>

> <span data-ttu-id="0db18-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0db18-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0db18-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0db18-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0db18-107">Stellt die Zuordnung zwischen einer Education Benutzertyp und der Domäne, der das Konto des Benutzers gehört.</span><span class="sxs-lookup"><span data-stu-id="0db18-107">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="0db18-108">Die Domänenressource ist Teil der [Identität Erstellung Konfiguration](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0db18-108">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="0db18-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0db18-109">Properties</span></span>

| <span data-ttu-id="0db18-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0db18-110">Property</span></span> | <span data-ttu-id="0db18-111">Typ</span><span class="sxs-lookup"><span data-stu-id="0db18-111">Type</span></span> | <span data-ttu-id="0db18-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0db18-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="0db18-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="0db18-113">**appliesTo**</span></span> | <span data-ttu-id="0db18-114">string</span><span class="sxs-lookup"><span data-stu-id="0db18-114">string</span></span> |  <span data-ttu-id="0db18-115">Der Benutzer Rollentyp Lizenz zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="0db18-115">The user role type to assign to license.</span></span> <span data-ttu-id="0db18-116">Mögliche Werte sind: `student` und `teacher`.</span><span class="sxs-lookup"><span data-stu-id="0db18-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="0db18-117">**name**</span><span class="sxs-lookup"><span data-stu-id="0db18-117">**name**</span></span> | <span data-ttu-id="0db18-118">string</span><span class="sxs-lookup"><span data-stu-id="0db18-118">string</span></span> |  <span data-ttu-id="0db18-119">Stellt die Domäne für das Benutzerkonto ein.</span><span class="sxs-lookup"><span data-stu-id="0db18-119">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="0db18-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0db18-120">JSON representation</span></span>
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
