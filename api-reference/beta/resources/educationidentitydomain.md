---
title: Ressourcentyp educationIdentityDomain
description: 'Stellt die Zuordnung zwischen einer Education Benutzertyp und der Domäne, der das Konto des Benutzers gehört. Die Domänenressource ist Teil der Identity-Konfiguration erstellen. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 280ae1a65e0c14e7960d316cc21154e405f2ee0d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982029"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="f77b4-104">Ressourcentyp educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="f77b4-104">educationIdentityDomain resource type</span></span>

> <span data-ttu-id="f77b4-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f77b4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f77b4-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f77b4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f77b4-107">Stellt die Zuordnung zwischen einer Education Benutzertyp und der Domäne, der das Konto des Benutzers gehört.</span><span class="sxs-lookup"><span data-stu-id="f77b4-107">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="f77b4-108">Die Domänenressource ist Teil der [Identität Erstellung Konfiguration](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f77b4-108">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="f77b4-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f77b4-109">Properties</span></span>

| <span data-ttu-id="f77b4-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f77b4-110">Property</span></span> | <span data-ttu-id="f77b4-111">Typ</span><span class="sxs-lookup"><span data-stu-id="f77b4-111">Type</span></span> | <span data-ttu-id="f77b4-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f77b4-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="f77b4-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="f77b4-113">**appliesTo**</span></span> | <span data-ttu-id="f77b4-114">string</span><span class="sxs-lookup"><span data-stu-id="f77b4-114">string</span></span> |  <span data-ttu-id="f77b4-115">Der Benutzer Rollentyp Lizenz zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="f77b4-115">The user role type to assign to license.</span></span> <span data-ttu-id="f77b4-116">Mögliche Werte sind: `student` und `teacher`.</span><span class="sxs-lookup"><span data-stu-id="f77b4-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="f77b4-117">**name**</span><span class="sxs-lookup"><span data-stu-id="f77b4-117">**name**</span></span> | <span data-ttu-id="f77b4-118">string</span><span class="sxs-lookup"><span data-stu-id="f77b4-118">string</span></span> |  <span data-ttu-id="f77b4-119">Stellt die Domäne für das Benutzerkonto ein.</span><span class="sxs-lookup"><span data-stu-id="f77b4-119">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="f77b4-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f77b4-120">JSON representation</span></span>
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
