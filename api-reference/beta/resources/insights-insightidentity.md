---
title: insightIdentity
description: Komplexer Typ, der Eigenschaften von gemeinsamen Elementen enthält.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 45ac8874a30ebb4f3196f03a675229bf1fab750c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523057"
---
# <a name="insightidentity"></a><span data-ttu-id="9b445-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="9b445-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b445-104">Komplexer Typ, der Eigenschaften von [gemeinsamen](insights-shared.md) Elementen enthält.</span><span class="sxs-lookup"><span data-stu-id="9b445-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="9b445-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9b445-105">JSON representation</span></span>
<span data-ttu-id="9b445-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9b445-106">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="9b445-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9b445-107">Properties</span></span>

| <span data-ttu-id="9b445-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9b445-108">Property</span></span>              | <span data-ttu-id="9b445-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9b445-109">Type</span></span>          | <span data-ttu-id="9b445-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9b445-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="9b445-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9b445-111">displayName</span></span>       | <span data-ttu-id="9b445-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9b445-112">String</span></span>          | <span data-ttu-id="9b445-113">Der Anzeigename des Benutzers, der das Element freigegeben.</span><span class="sxs-lookup"><span data-stu-id="9b445-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="9b445-114">id</span><span class="sxs-lookup"><span data-stu-id="9b445-114">id</span></span>              | <span data-ttu-id="9b445-115">string</span><span class="sxs-lookup"><span data-stu-id="9b445-115">String</span></span>        | <span data-ttu-id="9b445-116">Die Id des Benutzers, der das Element freigegeben.</span><span class="sxs-lookup"><span data-stu-id="9b445-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="9b445-117">address</span><span class="sxs-lookup"><span data-stu-id="9b445-117">address</span></span>             | <span data-ttu-id="9b445-118">String</span><span class="sxs-lookup"><span data-stu-id="9b445-118">String</span></span>      | <span data-ttu-id="9b445-119">Die e-Mail-Adresse des Benutzers, der das Element freigegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="9b445-119">The email address of the user who shared the item.</span></span>  |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-insightidentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
