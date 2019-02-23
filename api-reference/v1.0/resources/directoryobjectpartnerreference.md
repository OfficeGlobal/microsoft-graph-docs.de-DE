---
title: directoryObjectPartnerReference-Ressourcentyp
description: Stellt einen Verweis auf ein Directory-Objekt in einem Partner Mandanten dar. Erbt von directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0b84b7447d689759444e9cfd99982857eafa71eb
ms.sourcegitcommit: 7412dd2f2d5ed66afa2b0759c861ad23b4c6ecdf
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/23/2019
ms.locfileid: "30224129"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="40870-104">directoryObjectPartnerReference-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="40870-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="40870-105">Stellt einen Verweis auf ein Directory-Objekt in einer Partnerorganisation dar.</span><span class="sxs-lookup"><span data-stu-id="40870-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="40870-106">Erbt von [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="40870-106">Inherits from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span>

## <a name="properties"></a><span data-ttu-id="40870-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="40870-107">Properties</span></span>

| <span data-ttu-id="40870-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="40870-108">Property</span></span> | <span data-ttu-id="40870-109">Typ</span><span class="sxs-lookup"><span data-stu-id="40870-109">Type</span></span> | <span data-ttu-id="40870-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40870-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="40870-111">description</span><span class="sxs-lookup"><span data-stu-id="40870-111">description</span></span>|<span data-ttu-id="40870-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="40870-112">String</span></span>| <span data-ttu-id="40870-113">Beschreibung des zurückgegebenen Objekts.</span><span class="sxs-lookup"><span data-stu-id="40870-113">Description of the object returned.</span></span> <span data-ttu-id="40870-114">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="40870-114">Read-only.</span></span> |
|<span data-ttu-id="40870-115">displayName</span><span class="sxs-lookup"><span data-stu-id="40870-115">displayName</span></span>|<span data-ttu-id="40870-116">String</span><span class="sxs-lookup"><span data-stu-id="40870-116">String</span></span>| <span data-ttu-id="40870-117">Name des Verzeichnisobjekts, das zurückgegeben wird, wie Gruppe oder Anwendung.</span><span class="sxs-lookup"><span data-stu-id="40870-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="40870-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="40870-118">Read-only.</span></span> |
|<span data-ttu-id="40870-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="40870-119">externalPartnerTenantId</span></span>|<span data-ttu-id="40870-120">Guid</span><span class="sxs-lookup"><span data-stu-id="40870-120">Guid</span></span>| <span data-ttu-id="40870-121">Die Mandanten-ID für den Partner Mandanten.</span><span class="sxs-lookup"><span data-stu-id="40870-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="40870-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="40870-122">Read-only.</span></span> |
|<span data-ttu-id="40870-123">id</span><span class="sxs-lookup"><span data-stu-id="40870-123">id</span></span>|<span data-ttu-id="40870-124">string</span><span class="sxs-lookup"><span data-stu-id="40870-124">String</span></span>| <span data-ttu-id="40870-125">Der eindeutige Bezeichner für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="40870-125">The unique identifier for the resource.</span></span> <span data-ttu-id="40870-126">Geerbt von [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="40870-126">Inherited from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span> <span data-ttu-id="40870-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="40870-127">Read-only.</span></span> |
|<span data-ttu-id="40870-128">objectType</span><span class="sxs-lookup"><span data-stu-id="40870-128">objectType</span></span>|<span data-ttu-id="40870-129">String</span><span class="sxs-lookup"><span data-stu-id="40870-129">String</span></span>| <span data-ttu-id="40870-130">Der Typ des referenzierten Objekts im Partner Mandanten.</span><span class="sxs-lookup"><span data-stu-id="40870-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="40870-131">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="40870-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="40870-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="40870-132">JSON representation</span></span>

<span data-ttu-id="40870-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="40870-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObjectPartnerReference"
}-->

```json
{
  "description": "string ",
  "displayName": "string",
  "externalPartnerTenantId": "string (identifier)",
  "id": "string (identifier)",
  "objectType": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="40870-134">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="40870-134">See also</span></span>

- [<span data-ttu-id="40870-135">Directory-Objekte aus einer Liste von IDs abrufen</span><span class="sxs-lookup"><span data-stu-id="40870-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-v1.0)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryobjectpartnerreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
