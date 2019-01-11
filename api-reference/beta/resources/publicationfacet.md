---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
ms.openlocfilehash: 4cb3a56b5bdb4c3e7c9fc9fe69c0b34cae134a0d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805607"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="818c8-102">PublicationFacet-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="818c8-102">PublicationFacet resource type</span></span>

> <span data-ttu-id="818c8-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="818c8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="818c8-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="818c8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="818c8-105">Die **PublicationFacet**-Ressource enthält Details zum veröffentlichten Status einer [DriveItemVersion](driveitemversion.md)- oder [DriveItem](driveitem.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="818c8-105">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="818c8-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="818c8-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.publicationFacet"
}-->

```json
{
  "level": "published | checkout",
  "versionId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="818c8-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="818c8-107">Properties</span></span>

|   <span data-ttu-id="818c8-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="818c8-108">Property</span></span>    |  <span data-ttu-id="818c8-109">Typ</span><span class="sxs-lookup"><span data-stu-id="818c8-109">Type</span></span>  | <span data-ttu-id="818c8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="818c8-110">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="818c8-111">**level**</span><span class="sxs-lookup"><span data-stu-id="818c8-111">**level**</span></span>     | <span data-ttu-id="818c8-112">string</span><span class="sxs-lookup"><span data-stu-id="818c8-112">String</span></span> | <span data-ttu-id="818c8-113">Der Status der Veröffentlichung für dieses Dokument.</span><span class="sxs-lookup"><span data-stu-id="818c8-113">The state of publication for this document.</span></span> <span data-ttu-id="818c8-114">Möglich ist `published` oder `checkout`.</span><span class="sxs-lookup"><span data-stu-id="818c8-114">Either `published` or `checkout`.</span></span> <span data-ttu-id="818c8-115">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="818c8-115">Read-only.</span></span>  |
| <span data-ttu-id="818c8-116">**versionId**</span><span class="sxs-lookup"><span data-stu-id="818c8-116">**versionId**</span></span> | <span data-ttu-id="818c8-117">string</span><span class="sxs-lookup"><span data-stu-id="818c8-117">String</span></span> | <span data-ttu-id="818c8-118">Der eindeutige Bezeichner für die Version, die für den aktuellen Anrufer sichtbar ist.</span><span class="sxs-lookup"><span data-stu-id="818c8-118">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="818c8-119">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="818c8-119">Read-only.</span></span>  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
