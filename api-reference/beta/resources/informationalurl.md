---
title: Ressourcentyp informationalUrl
description: Grundlegende Profilinformationen der Anwendung.
localization_priority: Normal
ms.openlocfilehash: 5085c144045631c530cbb66f5e1f27186a63b380
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513648"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="418f0-103">Ressourcentyp informationalUrl</span><span class="sxs-lookup"><span data-stu-id="418f0-103">informationalUrl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="418f0-104">Grundlegende Profilinformationen der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="418f0-104">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="418f0-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="418f0-105">Properties</span></span>

| <span data-ttu-id="418f0-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="418f0-106">Property</span></span> | <span data-ttu-id="418f0-107">Typ</span><span class="sxs-lookup"><span data-stu-id="418f0-107">Type</span></span> | <span data-ttu-id="418f0-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="418f0-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="418f0-109">"Marketing"</span><span class="sxs-lookup"><span data-stu-id="418f0-109">marketing</span></span>|<span data-ttu-id="418f0-110">String</span><span class="sxs-lookup"><span data-stu-id="418f0-110">String</span></span>| <span data-ttu-id="418f0-111">Link zu marketing Anwendungsseite.</span><span class="sxs-lookup"><span data-stu-id="418f0-111">Link to the application's marketing page.</span></span> <span data-ttu-id="418f0-112">Beispiel: https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="418f0-112">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="418f0-113">Datenschutz</span><span class="sxs-lookup"><span data-stu-id="418f0-113">privacy</span></span>|<span data-ttu-id="418f0-114">String</span><span class="sxs-lookup"><span data-stu-id="418f0-114">String</span></span>| <span data-ttu-id="418f0-115">Link zu Datenschutzrichtlinie für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="418f0-115">Link to the application's privacy statement.</span></span> <span data-ttu-id="418f0-116">Beispiel: https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="418f0-116">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="418f0-117">Support</span><span class="sxs-lookup"><span data-stu-id="418f0-117">support</span></span>|<span data-ttu-id="418f0-118">String</span><span class="sxs-lookup"><span data-stu-id="418f0-118">String</span></span>| <span data-ttu-id="418f0-119">Link zu der Anwendung Supportseite.</span><span class="sxs-lookup"><span data-stu-id="418f0-119">Link to the application's support page.</span></span> <span data-ttu-id="418f0-120">Beispiel: https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="418f0-120">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="418f0-121">termsOfService</span><span class="sxs-lookup"><span data-stu-id="418f0-121">termsOfService</span></span>|<span data-ttu-id="418f0-122">String</span><span class="sxs-lookup"><span data-stu-id="418f0-122">String</span></span>| <span data-ttu-id="418f0-123">Link zu der Anwendung Begriffe der Service-Anweisung.</span><span class="sxs-lookup"><span data-stu-id="418f0-123">Link to the application's terms of service statement.</span></span> <span data-ttu-id="418f0-124">Beispiel: https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="418f0-124">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="418f0-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="418f0-125">JSON representation</span></span>
<span data-ttu-id="418f0-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="418f0-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationalUrl"
}-->

```json
{
  "marketing": "String",
  "privacy": "String",
  "support": "String",
  "termsOfService": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/informationalurl.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
