---
title: Ressourcentyp directoryObjectPartnerReference
description: Stellt einen Verweis auf ein Verzeichnisobjekt in einem Partner-Mandanten. Erbt von directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a031586d1f92bf2b8b331e9b71058211b4617382
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511051"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="33b47-104">Ressourcentyp directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="33b47-104">directoryObjectPartnerReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33b47-105">Stellt einen Verweis auf ein Verzeichnisobjekt in einer Partnerorganisation.</span><span class="sxs-lookup"><span data-stu-id="33b47-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="33b47-106">Erbt von [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="33b47-106">Inherits from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="33b47-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="33b47-107">Properties</span></span>

| <span data-ttu-id="33b47-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="33b47-108">Property</span></span> | <span data-ttu-id="33b47-109">Typ</span><span class="sxs-lookup"><span data-stu-id="33b47-109">Type</span></span> | <span data-ttu-id="33b47-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33b47-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="33b47-111">description</span><span class="sxs-lookup"><span data-stu-id="33b47-111">description</span></span>|<span data-ttu-id="33b47-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33b47-112">String</span></span>| <span data-ttu-id="33b47-113">Beschreibung des zurückgegebenen Objekts.</span><span class="sxs-lookup"><span data-stu-id="33b47-113">Description of the object returned.</span></span> <span data-ttu-id="33b47-114">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="33b47-114">Read-only.</span></span> |
|<span data-ttu-id="33b47-115">displayName</span><span class="sxs-lookup"><span data-stu-id="33b47-115">displayName</span></span>|<span data-ttu-id="33b47-116">String</span><span class="sxs-lookup"><span data-stu-id="33b47-116">String</span></span>| <span data-ttu-id="33b47-117">Name des Directory-Objekts zurückgegeben wird, wie die Gruppe oder eine andere Anwendung.</span><span class="sxs-lookup"><span data-stu-id="33b47-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="33b47-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="33b47-118">Read-only.</span></span> |
|<span data-ttu-id="33b47-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="33b47-119">externalPartnerTenantId</span></span>|<span data-ttu-id="33b47-120">Guid</span><span class="sxs-lookup"><span data-stu-id="33b47-120">Guid</span></span>| <span data-ttu-id="33b47-121">Die Mandanten-ID für den Mandanten Partner.</span><span class="sxs-lookup"><span data-stu-id="33b47-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="33b47-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="33b47-122">Read-only.</span></span> |
|<span data-ttu-id="33b47-123">id</span><span class="sxs-lookup"><span data-stu-id="33b47-123">id</span></span>|<span data-ttu-id="33b47-124">string</span><span class="sxs-lookup"><span data-stu-id="33b47-124">String</span></span>| <span data-ttu-id="33b47-125">Der eindeutige Bezeichner für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="33b47-125">The unique identifier for the resource.</span></span> <span data-ttu-id="33b47-126">Geerbt von [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="33b47-126">Inherited from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span> <span data-ttu-id="33b47-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="33b47-127">Read-only.</span></span> |
|<span data-ttu-id="33b47-128">objectType</span><span class="sxs-lookup"><span data-stu-id="33b47-128">objectType</span></span>|<span data-ttu-id="33b47-129">String</span><span class="sxs-lookup"><span data-stu-id="33b47-129">String</span></span>| <span data-ttu-id="33b47-130">Der Typ des Objekts im Mandanten Partner verwiesen wird.</span><span class="sxs-lookup"><span data-stu-id="33b47-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="33b47-131">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="33b47-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="33b47-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="33b47-132">JSON representation</span></span>

<span data-ttu-id="33b47-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="33b47-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="33b47-134">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="33b47-134">See also</span></span>

- <span data-ttu-id="33b47-135">Directory-Objekte aus einer Liste von IDs abrufen</span><span class="sxs-lookup"><span data-stu-id="33b47-135">[Get directory objects from a list of ids](/graph/api/directoryobject-getbyids?view=graph-rest-beta)</span></span>

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
