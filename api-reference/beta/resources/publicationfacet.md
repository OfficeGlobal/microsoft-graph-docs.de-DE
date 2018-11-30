---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: PublicationFacet
ms.openlocfilehash: 60dff1e0dd97073ccb7eccd7be0f51b6b77fc273
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062237"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="653dc-102">PublicationFacet-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="653dc-102">PublicationFacet resource type</span></span>

> <span data-ttu-id="653dc-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="653dc-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="653dc-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="653dc-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="653dc-105">Die **PublicationFacet**-Ressource enthält Details zum veröffentlichten Status einer [DriveItemVersion](driveitemversion.md)- oder [DriveItem](driveitem.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="653dc-105">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="653dc-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="653dc-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="653dc-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="653dc-107">Properties</span></span>

|   <span data-ttu-id="653dc-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="653dc-108">Property</span></span>    |  <span data-ttu-id="653dc-109">Typ</span><span class="sxs-lookup"><span data-stu-id="653dc-109">Type</span></span>  | <span data-ttu-id="653dc-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="653dc-110">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="653dc-111">**level**</span><span class="sxs-lookup"><span data-stu-id="653dc-111">**level**</span></span>     | <span data-ttu-id="653dc-112">string</span><span class="sxs-lookup"><span data-stu-id="653dc-112">String</span></span> | <span data-ttu-id="653dc-113">Der Status der Veröffentlichung für dieses Dokument.</span><span class="sxs-lookup"><span data-stu-id="653dc-113">The state of publication for this document.</span></span> <span data-ttu-id="653dc-114">Möglich ist `published` oder `checkout`.</span><span class="sxs-lookup"><span data-stu-id="653dc-114">Either `published` or `checkout`.</span></span> <span data-ttu-id="653dc-115">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="653dc-115">Read-only.</span></span>  |
| <span data-ttu-id="653dc-116">**versionId**</span><span class="sxs-lookup"><span data-stu-id="653dc-116">**versionId**</span></span> | <span data-ttu-id="653dc-117">string</span><span class="sxs-lookup"><span data-stu-id="653dc-117">String</span></span> | <span data-ttu-id="653dc-118">Der eindeutige Bezeichner für die Version, die für den aktuellen Anrufer sichtbar ist.</span><span class="sxs-lookup"><span data-stu-id="653dc-118">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="653dc-119">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="653dc-119">Read-only.</span></span>  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
