---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
ms.openlocfilehash: 9a5181e9cbc089832e8f73e0b8222ca63b69ca30
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894481"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="e51d4-102">BaseItemVersion-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e51d4-102">BaseItemVersion resource type</span></span>

> <span data-ttu-id="e51d4-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e51d4-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e51d4-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e51d4-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e51d4-105">Die **baseItemVersion**-Ressource stellt eine frühere Version eines Elements oder einer Entität dar.</span><span class="sxs-lookup"><span data-stu-id="e51d4-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e51d4-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e51d4-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e51d4-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e51d4-107">Properties</span></span>

|      <span data-ttu-id="e51d4-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="e51d4-108">Property name</span></span>       |                         <span data-ttu-id="e51d4-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e51d4-109">Type</span></span>                         |                               <span data-ttu-id="e51d4-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e51d4-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="e51d4-111">**id**</span><span class="sxs-lookup"><span data-stu-id="e51d4-111">**id**</span></span>                   | <span data-ttu-id="e51d4-112">string</span><span class="sxs-lookup"><span data-stu-id="e51d4-112">string</span></span>                                               | <span data-ttu-id="e51d4-113">Die ID der Version.</span><span class="sxs-lookup"><span data-stu-id="e51d4-113">The ID of the version.</span></span> <span data-ttu-id="e51d4-114">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e51d4-114">Read-only.</span></span>                                       |
| <span data-ttu-id="e51d4-115">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="e51d4-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="e51d4-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="e51d4-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="e51d4-117">Die Identität des Benutzers, der die Version zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="e51d4-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="e51d4-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e51d4-118">Read-only.</span></span>        |
| <span data-ttu-id="e51d4-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="e51d4-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="e51d4-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e51d4-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="e51d4-121">Datum und Uhrzeit der letzten Änderung der Version.</span><span class="sxs-lookup"><span data-stu-id="e51d4-121">Date and time the version was last modified.</span></span> <span data-ttu-id="e51d4-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e51d4-122">Read-only.</span></span>                 |
| <span data-ttu-id="e51d4-123">**Veröffentlichung**</span><span class="sxs-lookup"><span data-stu-id="e51d4-123">**publication**</span></span>          | [<span data-ttu-id="e51d4-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="e51d4-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="e51d4-125">Zeigt den Veröffentlichungsstatus dieser bestimmten Version an.</span><span class="sxs-lookup"><span data-stu-id="e51d4-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="e51d4-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e51d4-126">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
