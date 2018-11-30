---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: BaseItemVersion
ms.openlocfilehash: dfda19af6057bc1d6e1757d24f6a2c99979a8622
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058140"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="2087a-102">BaseItemVersion-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2087a-102">BaseItemVersion resource type</span></span>

> <span data-ttu-id="2087a-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2087a-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2087a-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2087a-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2087a-105">Die **baseItemVersion**-Ressource stellt eine frühere Version eines Elements oder einer Entität dar.</span><span class="sxs-lookup"><span data-stu-id="2087a-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="2087a-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2087a-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2087a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2087a-107">Properties</span></span>

|      <span data-ttu-id="2087a-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="2087a-108">Property name</span></span>       |                         <span data-ttu-id="2087a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="2087a-109">Type</span></span>                         |                               <span data-ttu-id="2087a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2087a-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="2087a-111">**id**</span><span class="sxs-lookup"><span data-stu-id="2087a-111">**id**</span></span>                   | <span data-ttu-id="2087a-112">string</span><span class="sxs-lookup"><span data-stu-id="2087a-112">string</span></span>                                               | <span data-ttu-id="2087a-113">Die ID der Version.</span><span class="sxs-lookup"><span data-stu-id="2087a-113">The ID of the version.</span></span> <span data-ttu-id="2087a-114">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2087a-114">Read-only.</span></span>                                       |
| <span data-ttu-id="2087a-115">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="2087a-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="2087a-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="2087a-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="2087a-117">Die Identität des Benutzers, der die Version zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="2087a-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="2087a-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2087a-118">Read-only.</span></span>        |
| <span data-ttu-id="2087a-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="2087a-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="2087a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2087a-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="2087a-121">Datum und Uhrzeit der letzten Änderung der Version.</span><span class="sxs-lookup"><span data-stu-id="2087a-121">Date and time the version was last modified.</span></span> <span data-ttu-id="2087a-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2087a-122">Read-only.</span></span>                 |
| <span data-ttu-id="2087a-123">**Veröffentlichung**</span><span class="sxs-lookup"><span data-stu-id="2087a-123">**publication**</span></span>          | [<span data-ttu-id="2087a-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="2087a-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="2087a-125">Zeigt den Veröffentlichungsstatus dieser bestimmten Version an.</span><span class="sxs-lookup"><span data-stu-id="2087a-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="2087a-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2087a-126">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->