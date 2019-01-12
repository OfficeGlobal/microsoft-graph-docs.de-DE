---
title: Ressourcentyp oneNoteIdentity
description: '**Unterstützung in Kürze verfügbar**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7ce71775842cc6b7084b86e13e9e4715765567ac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963213"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="275ab-103">Ressourcentyp oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="275ab-103">oneNoteIdentity resource type</span></span>

> <span data-ttu-id="275ab-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="275ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="275ab-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="275ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="275ab-106">**Unterstützung in Kürze verfügbar**</span><span class="sxs-lookup"><span data-stu-id="275ab-106">**Support coming soon**</span></span>

<span data-ttu-id="275ab-107">Der Typ OneNoteIdentity stellt eine Identität eines _Benutzers_.</span><span class="sxs-lookup"><span data-stu-id="275ab-107">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="275ab-108">In Zukunft werden sollen dieses Typs mit [Identität](identity.md) zusammengeführt</span><span class="sxs-lookup"><span data-stu-id="275ab-108">In future, this type will be merged with [Identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="275ab-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="275ab-109">JSON representation</span></span>

<span data-ttu-id="275ab-110">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="275ab-110">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}

```
## <a name="properties"></a><span data-ttu-id="275ab-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="275ab-111">Properties</span></span>
| <span data-ttu-id="275ab-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="275ab-112">Property</span></span>     | <span data-ttu-id="275ab-113">Typ</span><span class="sxs-lookup"><span data-stu-id="275ab-113">Type</span></span>   |<span data-ttu-id="275ab-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="275ab-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="275ab-115">displayName</span><span class="sxs-lookup"><span data-stu-id="275ab-115">displayName</span></span>|<span data-ttu-id="275ab-116">string</span><span class="sxs-lookup"><span data-stu-id="275ab-116">string</span></span>|<span data-ttu-id="275ab-117">Die Identität der Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="275ab-117">The identity's display name.</span></span>|
|<span data-ttu-id="275ab-118">id</span><span class="sxs-lookup"><span data-stu-id="275ab-118">id</span></span>|<span data-ttu-id="275ab-119">string</span><span class="sxs-lookup"><span data-stu-id="275ab-119">string</span></span>|<span data-ttu-id="275ab-120">Eindeutiger Bezeichner für die Identität.</span><span class="sxs-lookup"><span data-stu-id="275ab-120">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
