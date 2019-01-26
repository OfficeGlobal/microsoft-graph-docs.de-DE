---
title: Ressourcentyp oneNoteIdentity
description: '**Unterstützung in Kürze verfügbar**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 33cb7d63ab103723ae5bb8d24c19add4bb7ef5ac
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576878"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="e98d8-103">Ressourcentyp oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="e98d8-103">oneNoteIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e98d8-104">**Unterstützung in Kürze verfügbar**</span><span class="sxs-lookup"><span data-stu-id="e98d8-104">**Support coming soon**</span></span>

<span data-ttu-id="e98d8-105">Der Typ OneNoteIdentity stellt eine Identität eines _Benutzers_.</span><span class="sxs-lookup"><span data-stu-id="e98d8-105">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="e98d8-106">In Zukunft werden sollen dieses Typs mit [Identität](identity.md) zusammengeführt</span><span class="sxs-lookup"><span data-stu-id="e98d8-106">In future, this type will be merged with [Identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="e98d8-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e98d8-107">JSON representation</span></span>

<span data-ttu-id="e98d8-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e98d8-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oneNoteIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}

```
## <a name="properties"></a><span data-ttu-id="e98d8-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e98d8-109">Properties</span></span>
| <span data-ttu-id="e98d8-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e98d8-110">Property</span></span>     | <span data-ttu-id="e98d8-111">Typ</span><span class="sxs-lookup"><span data-stu-id="e98d8-111">Type</span></span>   |<span data-ttu-id="e98d8-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e98d8-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e98d8-113">displayName</span><span class="sxs-lookup"><span data-stu-id="e98d8-113">displayName</span></span>|<span data-ttu-id="e98d8-114">string</span><span class="sxs-lookup"><span data-stu-id="e98d8-114">string</span></span>|<span data-ttu-id="e98d8-115">Die Identität der Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="e98d8-115">The identity's display name.</span></span>|
|<span data-ttu-id="e98d8-116">id</span><span class="sxs-lookup"><span data-stu-id="e98d8-116">id</span></span>|<span data-ttu-id="e98d8-117">string</span><span class="sxs-lookup"><span data-stu-id="e98d8-117">string</span></span>|<span data-ttu-id="e98d8-118">Eindeutiger Bezeichner für die Identität.</span><span class="sxs-lookup"><span data-stu-id="e98d8-118">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteidentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
