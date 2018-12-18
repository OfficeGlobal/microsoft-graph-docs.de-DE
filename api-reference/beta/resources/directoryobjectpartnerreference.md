---
title: Ressourcentyp directoryObjectPartnerReference
description: Stellt einen Verweis auf ein Verzeichnisobjekt in einem Partner-Mandanten. Erbt von directoryObject.
author: lleonard-msft
ms.openlocfilehash: 37a60c126ef74f3073f258ba799cf276fda4f5cf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336946"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="afb91-104">Ressourcentyp directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="afb91-104">directoryObjectPartnerReference resource type</span></span>

> <span data-ttu-id="afb91-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="afb91-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="afb91-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="afb91-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="afb91-107">Stellt einen Verweis auf ein Verzeichnisobjekt in einer Partnerorganisation.</span><span class="sxs-lookup"><span data-stu-id="afb91-107">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="afb91-108">Erbt von [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="afb91-108">Inherits from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="afb91-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="afb91-109">Properties</span></span>

| <span data-ttu-id="afb91-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="afb91-110">Property</span></span> | <span data-ttu-id="afb91-111">Typ</span><span class="sxs-lookup"><span data-stu-id="afb91-111">Type</span></span> | <span data-ttu-id="afb91-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="afb91-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="afb91-113">description</span><span class="sxs-lookup"><span data-stu-id="afb91-113">description</span></span>|<span data-ttu-id="afb91-114">String</span><span class="sxs-lookup"><span data-stu-id="afb91-114">String</span></span>| <span data-ttu-id="afb91-115">Beschreibung des zurückgegebenen Objekts.</span><span class="sxs-lookup"><span data-stu-id="afb91-115">Description of the object returned.</span></span> <span data-ttu-id="afb91-116">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="afb91-116">Read-only.</span></span> |
|<span data-ttu-id="afb91-117">displayName</span><span class="sxs-lookup"><span data-stu-id="afb91-117">displayName</span></span>|<span data-ttu-id="afb91-118">String</span><span class="sxs-lookup"><span data-stu-id="afb91-118">String</span></span>| <span data-ttu-id="afb91-119">Name des Directory-Objekts zurückgegeben wird, wie die Gruppe oder eine andere Anwendung.</span><span class="sxs-lookup"><span data-stu-id="afb91-119">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="afb91-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="afb91-120">Read-only.</span></span> |
|<span data-ttu-id="afb91-121">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="afb91-121">externalPartnerTenantId</span></span>|<span data-ttu-id="afb91-122">Guid</span><span class="sxs-lookup"><span data-stu-id="afb91-122">Guid</span></span>| <span data-ttu-id="afb91-123">Die Mandanten-ID für den Mandanten Partner.</span><span class="sxs-lookup"><span data-stu-id="afb91-123">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="afb91-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="afb91-124">Read-only.</span></span> |
|<span data-ttu-id="afb91-125">id</span><span class="sxs-lookup"><span data-stu-id="afb91-125">id</span></span>|<span data-ttu-id="afb91-126">String</span><span class="sxs-lookup"><span data-stu-id="afb91-126">String</span></span>| <span data-ttu-id="afb91-127">Der eindeutige Bezeichner für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="afb91-127">The unique identifier for the resource.</span></span> <span data-ttu-id="afb91-128">Geerbt von [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="afb91-128">Inherited from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span> <span data-ttu-id="afb91-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="afb91-129">Read-only.</span></span> |
|<span data-ttu-id="afb91-130">objectType</span><span class="sxs-lookup"><span data-stu-id="afb91-130">objectType</span></span>|<span data-ttu-id="afb91-131">String</span><span class="sxs-lookup"><span data-stu-id="afb91-131">String</span></span>| <span data-ttu-id="afb91-132">Der Typ des Objekts im Mandanten Partner verwiesen wird.</span><span class="sxs-lookup"><span data-stu-id="afb91-132">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="afb91-133">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="afb91-133">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="afb91-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="afb91-134">JSON representation</span></span>

<span data-ttu-id="afb91-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="afb91-135">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="afb91-136">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="afb91-136">See also</span></span>

- [<span data-ttu-id="afb91-137">Directory-Objekte aus einer Liste von IDs abrufen</span><span class="sxs-lookup"><span data-stu-id="afb91-137">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
