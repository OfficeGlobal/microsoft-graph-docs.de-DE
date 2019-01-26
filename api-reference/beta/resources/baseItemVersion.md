---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
ms.openlocfilehash: 92784fd9836c0ffd8fe748c2daee0947edefbbdc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571107"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="739e1-102">BaseItemVersion-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="739e1-102">BaseItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="739e1-103">Die **baseItemVersion**-Ressource stellt eine frühere Version eines Elements oder einer Entität dar.</span><span class="sxs-lookup"><span data-stu-id="739e1-103">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="739e1-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="739e1-104">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="739e1-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="739e1-105">Properties</span></span>

|      <span data-ttu-id="739e1-106">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="739e1-106">Property name</span></span>       |                         <span data-ttu-id="739e1-107">Typ</span><span class="sxs-lookup"><span data-stu-id="739e1-107">Type</span></span>                         |                               <span data-ttu-id="739e1-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="739e1-108">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="739e1-109">**id**</span><span class="sxs-lookup"><span data-stu-id="739e1-109">**id**</span></span>                   | <span data-ttu-id="739e1-110">string</span><span class="sxs-lookup"><span data-stu-id="739e1-110">string</span></span>                                               | <span data-ttu-id="739e1-111">Die ID der Version.</span><span class="sxs-lookup"><span data-stu-id="739e1-111">The ID of the version.</span></span> <span data-ttu-id="739e1-112">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="739e1-112">Read-only.</span></span>                                       |
| <span data-ttu-id="739e1-113">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="739e1-113">**lastModifiedBy**</span></span>       | [<span data-ttu-id="739e1-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="739e1-114">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="739e1-115">Die Identität des Benutzers, der die Version zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="739e1-115">Identity of the user which last modified the version.</span></span> <span data-ttu-id="739e1-116">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="739e1-116">Read-only.</span></span>        |
| <span data-ttu-id="739e1-117">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="739e1-117">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="739e1-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="739e1-118">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="739e1-119">Datum und Uhrzeit der letzten Änderung der Version.</span><span class="sxs-lookup"><span data-stu-id="739e1-119">Date and time the version was last modified.</span></span> <span data-ttu-id="739e1-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="739e1-120">Read-only.</span></span>                 |
| <span data-ttu-id="739e1-121">**Veröffentlichung**</span><span class="sxs-lookup"><span data-stu-id="739e1-121">**publication**</span></span>          | [<span data-ttu-id="739e1-122">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="739e1-122">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="739e1-123">Zeigt den Veröffentlichungsstatus dieser bestimmten Version an.</span><span class="sxs-lookup"><span data-stu-id="739e1-123">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="739e1-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="739e1-124">Read-only.</span></span> |


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
