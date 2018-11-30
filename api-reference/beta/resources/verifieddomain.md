---
title: verifiedDomain-Ressourcentyp
description: Gibt eine Domäne für einen Mandanten an. Die **verifiedDomains**-Eigenschaft der organization-Entität ist eine Auflistung von **VerifiedDomain**.
ms.openlocfilehash: 810b5fea0fbaf82eeb452c0f5c6032679590ff49
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063431"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="a582b-104">verifiedDomain-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a582b-104">verifiedDomain resource type</span></span>

> <span data-ttu-id="a582b-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a582b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a582b-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a582b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a582b-p103">Gibt eine Domäne für einen Mandanten an. Die **verifiedDomains**-Eigenschaft der [organization](organization.md)-Entität ist eine Auflistung von **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="a582b-p103">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="a582b-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a582b-109">Properties</span></span>
| <span data-ttu-id="a582b-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a582b-110">Property</span></span>     | <span data-ttu-id="a582b-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a582b-111">Type</span></span>   |<span data-ttu-id="a582b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a582b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a582b-113">Funktionen</span><span class="sxs-lookup"><span data-stu-id="a582b-113">capabilities</span></span>|<span data-ttu-id="a582b-114">String</span><span class="sxs-lookup"><span data-stu-id="a582b-114">String</span></span>|<span data-ttu-id="a582b-115">Zum Beispiel „Email“, „OfficeCommunicationsOnline“.</span><span class="sxs-lookup"><span data-stu-id="a582b-115">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="a582b-116">isDefault</span><span class="sxs-lookup"><span data-stu-id="a582b-116">isDefault</span></span>|<span data-ttu-id="a582b-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="a582b-117">Boolean</span></span>|                <span data-ttu-id="a582b-118">**true**, wenn dies die Standarddomäne ist, die dem Mandanten zugeordnet ist, andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="a582b-118">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="a582b-119">isInitial</span><span class="sxs-lookup"><span data-stu-id="a582b-119">isInitial</span></span>|<span data-ttu-id="a582b-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="a582b-120">Boolean</span></span>|<span data-ttu-id="a582b-121">**true**, wenn dies die ursprüngliche Domäne ist, die dem Mandanten zugeordnet ist, andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="a582b-121">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="a582b-122">name</span><span class="sxs-lookup"><span data-stu-id="a582b-122">name</span></span>|<span data-ttu-id="a582b-123">String</span><span class="sxs-lookup"><span data-stu-id="a582b-123">String</span></span>|<span data-ttu-id="a582b-124">Der Domänenname, zum Beispiel „contoso.onmicrosoft.com“</span><span class="sxs-lookup"><span data-stu-id="a582b-124">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="a582b-125">type</span><span class="sxs-lookup"><span data-stu-id="a582b-125">type</span></span>|<span data-ttu-id="a582b-126">String</span><span class="sxs-lookup"><span data-stu-id="a582b-126">String</span></span>|<span data-ttu-id="a582b-127">Z. B. „verwaltet“.</span><span class="sxs-lookup"><span data-stu-id="a582b-127">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a582b-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a582b-128">JSON representation</span></span>

<span data-ttu-id="a582b-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a582b-129">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifieddomain"
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
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
