---
title: Ressourcentyp informationalUrl
description: Grundlegende Profilinformationen der Anwendung.
localization_priority: Normal
ms.openlocfilehash: 78fd03a2673b342d1a0c904f521fe5a0f8cba205
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816982"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="a3c75-103">Ressourcentyp informationalUrl</span><span class="sxs-lookup"><span data-stu-id="a3c75-103">informationalUrl resource type</span></span>

> <span data-ttu-id="a3c75-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a3c75-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3c75-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a3c75-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a3c75-106">Grundlegende Profilinformationen der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="a3c75-106">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="a3c75-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a3c75-107">Properties</span></span>

| <span data-ttu-id="a3c75-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a3c75-108">Property</span></span> | <span data-ttu-id="a3c75-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a3c75-109">Type</span></span> | <span data-ttu-id="a3c75-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a3c75-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a3c75-111">"Marketing"</span><span class="sxs-lookup"><span data-stu-id="a3c75-111">marketing</span></span>|<span data-ttu-id="a3c75-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3c75-112">String</span></span>| <span data-ttu-id="a3c75-113">Link zu marketing Anwendungsseite.</span><span class="sxs-lookup"><span data-stu-id="a3c75-113">Link to the application's marketing page.</span></span> <span data-ttu-id="a3c75-114">Beispielsweise gibt https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="a3c75-114">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="a3c75-115">Datenschutz</span><span class="sxs-lookup"><span data-stu-id="a3c75-115">privacy</span></span>|<span data-ttu-id="a3c75-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3c75-116">String</span></span>| <span data-ttu-id="a3c75-117">Link zu Datenschutzrichtlinie für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="a3c75-117">Link to the application's privacy statement.</span></span> <span data-ttu-id="a3c75-118">Beispielsweise gibt https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="a3c75-118">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="a3c75-119">Unterstützung</span><span class="sxs-lookup"><span data-stu-id="a3c75-119">support</span></span>|<span data-ttu-id="a3c75-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3c75-120">String</span></span>| <span data-ttu-id="a3c75-121">Link zu der Anwendung Supportseite.</span><span class="sxs-lookup"><span data-stu-id="a3c75-121">Link to the application's support page.</span></span> <span data-ttu-id="a3c75-122">Beispielsweise gibt https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="a3c75-122">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="a3c75-123">termsOfService</span><span class="sxs-lookup"><span data-stu-id="a3c75-123">termsOfService</span></span>|<span data-ttu-id="a3c75-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3c75-124">String</span></span>| <span data-ttu-id="a3c75-125">Link zu der Anwendung Begriffe der Service-Anweisung.</span><span class="sxs-lookup"><span data-stu-id="a3c75-125">Link to the application's terms of service statement.</span></span> <span data-ttu-id="a3c75-126">Beispielsweise gibt https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="a3c75-126">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a3c75-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a3c75-127">JSON representation</span></span>
<span data-ttu-id="a3c75-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a3c75-128">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
