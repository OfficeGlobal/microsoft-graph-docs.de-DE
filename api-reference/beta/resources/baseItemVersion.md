---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
ms.openlocfilehash: fcf427300007277f7ea6382579ad3a0929ca97d1
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643024"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="89c09-102">BaseItemVersion-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="89c09-102">BaseItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89c09-103">Die **baseItemVersion**-Ressource stellt eine frühere Version eines Elements oder einer Entität dar.</span><span class="sxs-lookup"><span data-stu-id="89c09-103">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="89c09-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="89c09-104">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.baseItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="89c09-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="89c09-105">Properties</span></span>

|      <span data-ttu-id="89c09-106">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="89c09-106">Property name</span></span>       |                         <span data-ttu-id="89c09-107">Typ</span><span class="sxs-lookup"><span data-stu-id="89c09-107">Type</span></span>                         |                               <span data-ttu-id="89c09-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="89c09-108">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="89c09-109">**id**</span><span class="sxs-lookup"><span data-stu-id="89c09-109">**id**</span></span>                   | <span data-ttu-id="89c09-110">string</span><span class="sxs-lookup"><span data-stu-id="89c09-110">string</span></span>                                               | <span data-ttu-id="89c09-111">Die ID der Version.</span><span class="sxs-lookup"><span data-stu-id="89c09-111">The ID of the version.</span></span> <span data-ttu-id="89c09-112">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="89c09-112">Read-only.</span></span>                                       |
| <span data-ttu-id="89c09-113">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="89c09-113">**lastModifiedBy**</span></span>       | [<span data-ttu-id="89c09-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="89c09-114">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="89c09-115">Die Identität des Benutzers, der die Version zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="89c09-115">Identity of the user which last modified the version.</span></span> <span data-ttu-id="89c09-116">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="89c09-116">Read-only.</span></span>        |
| <span data-ttu-id="89c09-117">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="89c09-117">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="89c09-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89c09-118">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="89c09-119">Datum und Uhrzeit der letzten Änderung der Version.</span><span class="sxs-lookup"><span data-stu-id="89c09-119">Date and time the version was last modified.</span></span> <span data-ttu-id="89c09-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="89c09-120">Read-only.</span></span>                 |
| <span data-ttu-id="89c09-121">**Veröffentlichung**</span><span class="sxs-lookup"><span data-stu-id="89c09-121">**publication**</span></span>          | [<span data-ttu-id="89c09-122">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="89c09-122">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="89c09-123">Zeigt den Veröffentlichungsstatus dieser bestimmten Version an.</span><span class="sxs-lookup"><span data-stu-id="89c09-123">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="89c09-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="89c09-124">Read-only.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/baseItemVersion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
