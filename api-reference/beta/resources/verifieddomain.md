---
title: verifiedDomain-Ressourcentyp
description: Gibt eine Domäne für einen Mandanten an. Die **verifiedDomains**-Eigenschaft der organization-Entität ist eine Auflistung von **VerifiedDomain**.
localization_priority: Normal
ms.openlocfilehash: 01e2d174f47d08bea4de9d582ffd6126002e8f1f
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576871"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="143c3-104">verifiedDomain-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="143c3-104">verifiedDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="143c3-p102">Gibt eine Domäne für einen Mandanten an. Die **verifiedDomains**-Eigenschaft der [organization](organization.md)-Entität ist eine Auflistung von **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="143c3-p102">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="143c3-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="143c3-107">Properties</span></span>
| <span data-ttu-id="143c3-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="143c3-108">Property</span></span>     | <span data-ttu-id="143c3-109">Typ</span><span class="sxs-lookup"><span data-stu-id="143c3-109">Type</span></span>   |<span data-ttu-id="143c3-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="143c3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="143c3-111">Funktionen</span><span class="sxs-lookup"><span data-stu-id="143c3-111">capabilities</span></span>|<span data-ttu-id="143c3-112">String</span><span class="sxs-lookup"><span data-stu-id="143c3-112">String</span></span>|<span data-ttu-id="143c3-113">Zum Beispiel „Email“, „OfficeCommunicationsOnline“.</span><span class="sxs-lookup"><span data-stu-id="143c3-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="143c3-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="143c3-114">isDefault</span></span>|<span data-ttu-id="143c3-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="143c3-115">Boolean</span></span>|                <span data-ttu-id="143c3-116">**true**, wenn dies die Standarddomäne ist, die dem Mandanten zugeordnet ist, andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="143c3-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="143c3-117">isInitial</span><span class="sxs-lookup"><span data-stu-id="143c3-117">isInitial</span></span>|<span data-ttu-id="143c3-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="143c3-118">Boolean</span></span>|<span data-ttu-id="143c3-119">**true**, wenn dies die ursprüngliche Domäne ist, die dem Mandanten zugeordnet ist, andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="143c3-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="143c3-120">name</span><span class="sxs-lookup"><span data-stu-id="143c3-120">name</span></span>|<span data-ttu-id="143c3-121">String</span><span class="sxs-lookup"><span data-stu-id="143c3-121">String</span></span>|<span data-ttu-id="143c3-122">Der Domänenname, zum Beispiel „contoso.onmicrosoft.com“</span><span class="sxs-lookup"><span data-stu-id="143c3-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="143c3-123">type</span><span class="sxs-lookup"><span data-stu-id="143c3-123">type</span></span>|<span data-ttu-id="143c3-124">String</span><span class="sxs-lookup"><span data-stu-id="143c3-124">String</span></span>|<span data-ttu-id="143c3-125">Z. B. „verwaltet“.</span><span class="sxs-lookup"><span data-stu-id="143c3-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="143c3-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="143c3-126">JSON representation</span></span>

<span data-ttu-id="143c3-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="143c3-127">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedDomain"
}-->

```json
{
  "capabilities": "string",
  "isDefault": true,
  "isInitial": true,
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/verifieddomain.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
