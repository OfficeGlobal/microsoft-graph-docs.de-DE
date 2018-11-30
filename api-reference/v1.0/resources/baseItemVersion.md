---
title: BaseItemVersion-Ressourcentyp
description: Die **baseItemVersion**-Ressource stellt eine frühere Version eines Elements oder einer Entität dar.
ms.openlocfilehash: c4fc95fd419bf8b2f20ab202874ca31a2b1d63f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017502"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="b4c58-103">BaseItemVersion-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b4c58-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="b4c58-104">Die **baseItemVersion**-Ressource stellt eine frühere Version eines Elements oder einer Entität dar.</span><span class="sxs-lookup"><span data-stu-id="b4c58-104">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b4c58-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b4c58-105">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="b4c58-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b4c58-106">Properties</span></span>

|      <span data-ttu-id="b4c58-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="b4c58-107">Property name</span></span>       |                         <span data-ttu-id="b4c58-108">Typ</span><span class="sxs-lookup"><span data-stu-id="b4c58-108">Type</span></span>                         |                               <span data-ttu-id="b4c58-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4c58-109">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="b4c58-110">**id**</span><span class="sxs-lookup"><span data-stu-id="b4c58-110">**id**</span></span>                   | <span data-ttu-id="b4c58-111">string</span><span class="sxs-lookup"><span data-stu-id="b4c58-111">string</span></span>                                               | <span data-ttu-id="b4c58-112">Die ID der Version.</span><span class="sxs-lookup"><span data-stu-id="b4c58-112">The ID of the version.</span></span> <span data-ttu-id="b4c58-113">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b4c58-113">Read-only.</span></span>                                       |
| <span data-ttu-id="b4c58-114">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="b4c58-114">**lastModifiedBy**</span></span>       | [<span data-ttu-id="b4c58-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="b4c58-115">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="b4c58-116">Die Identität des Benutzers, der die Version zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="b4c58-116">Identity of the user which last modified the version.</span></span> <span data-ttu-id="b4c58-117">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b4c58-117">Read-only.</span></span>        |
| <span data-ttu-id="b4c58-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="b4c58-118">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="b4c58-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4c58-119">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="b4c58-120">Datum und Uhrzeit der letzten Änderung der Version.</span><span class="sxs-lookup"><span data-stu-id="b4c58-120">Date and time the version was last modified.</span></span> <span data-ttu-id="b4c58-121">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b4c58-121">Read-only.</span></span>                 |
| <span data-ttu-id="b4c58-122">**Veröffentlichung**</span><span class="sxs-lookup"><span data-stu-id="b4c58-122">**publication**</span></span>          | [<span data-ttu-id="b4c58-123">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="b4c58-123">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="b4c58-124">Zeigt den Veröffentlichungsstatus dieser bestimmten Version an.</span><span class="sxs-lookup"><span data-stu-id="b4c58-124">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="b4c58-125">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b4c58-125">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
