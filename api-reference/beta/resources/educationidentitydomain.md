---
title: Ressourcentyp educationIdentityDomain
description: 'Stellt die Zuordnung zwischen einer Education Benutzertyp und der Domäne, der das Konto des Benutzers gehört. Die Domänenressource ist Teil der Identity-Konfiguration erstellen. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 4eb9e5b58f62a23dbe1b450c2ec6b9d2f94970ac
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395650"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="074a9-104">Ressourcentyp educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="074a9-104">educationIdentityDomain resource type</span></span>

> <span data-ttu-id="074a9-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="074a9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="074a9-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="074a9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="074a9-107">Stellt die Zuordnung zwischen einer Education Benutzertyp und der Domäne, der das Konto des Benutzers gehört.</span><span class="sxs-lookup"><span data-stu-id="074a9-107">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="074a9-108">Die Domänenressource ist Teil der [Identität Erstellung Konfiguration](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="074a9-108">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="074a9-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="074a9-109">Properties</span></span>

| <span data-ttu-id="074a9-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="074a9-110">Property</span></span> | <span data-ttu-id="074a9-111">Typ</span><span class="sxs-lookup"><span data-stu-id="074a9-111">Type</span></span> | <span data-ttu-id="074a9-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="074a9-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="074a9-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="074a9-113">**appliesTo**</span></span> | <span data-ttu-id="074a9-114">string</span><span class="sxs-lookup"><span data-stu-id="074a9-114">string</span></span> |  <span data-ttu-id="074a9-115">Der Benutzer Rollentyp Lizenz zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="074a9-115">The user role type to assign to license.</span></span> <span data-ttu-id="074a9-116">Mögliche Werte sind: `student` und `teacher`.</span><span class="sxs-lookup"><span data-stu-id="074a9-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="074a9-117">**name**</span><span class="sxs-lookup"><span data-stu-id="074a9-117">**name**</span></span> | <span data-ttu-id="074a9-118">string</span><span class="sxs-lookup"><span data-stu-id="074a9-118">string</span></span> |  <span data-ttu-id="074a9-119">Stellt die Domäne für das Benutzerkonto ein.</span><span class="sxs-lookup"><span data-stu-id="074a9-119">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="074a9-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="074a9-120">JSON representation</span></span>
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
