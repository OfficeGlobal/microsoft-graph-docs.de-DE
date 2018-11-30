---
title: Empfänger Ressourcentyp
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: aa620fa920b4f91b2b2214f02c2e75d7a8cbcc4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064868"
---
# <a name="recipients-resource-type"></a><span data-ttu-id="faac4-103">Empfänger Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="faac4-103">recipients resource type</span></span>

> <span data-ttu-id="faac4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="faac4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="faac4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="faac4-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="faac4-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="faac4-106">JSON representation</span></span>

<span data-ttu-id="faac4-107">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="faac4-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipients"
}-->

```json
{
  "alias": "string",
  "email": "string",
  "objectId": "string",
  "permissionIdentityType": "string"
}

```
## <a name="properties"></a><span data-ttu-id="faac4-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="faac4-108">Properties</span></span>
| <span data-ttu-id="faac4-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="faac4-109">Property</span></span>     | <span data-ttu-id="faac4-110">Typ</span><span class="sxs-lookup"><span data-stu-id="faac4-110">Type</span></span>   |<span data-ttu-id="faac4-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="faac4-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="faac4-112">Alias</span><span class="sxs-lookup"><span data-stu-id="faac4-112">alias</span></span>|<span data-ttu-id="faac4-113">String</span><span class="sxs-lookup"><span data-stu-id="faac4-113">String</span></span>||
|<span data-ttu-id="faac4-114">E-Mail</span><span class="sxs-lookup"><span data-stu-id="faac4-114">email</span></span>|<span data-ttu-id="faac4-115">String</span><span class="sxs-lookup"><span data-stu-id="faac4-115">String</span></span>||
|<span data-ttu-id="faac4-116">objectId</span><span class="sxs-lookup"><span data-stu-id="faac4-116">objectId</span></span>|<span data-ttu-id="faac4-117">String</span><span class="sxs-lookup"><span data-stu-id="faac4-117">String</span></span>||
|<span data-ttu-id="faac4-118">permissionIdentityType</span><span class="sxs-lookup"><span data-stu-id="faac4-118">permissionIdentityType</span></span>|<span data-ttu-id="faac4-119">String</span><span class="sxs-lookup"><span data-stu-id="faac4-119">String</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipients resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->