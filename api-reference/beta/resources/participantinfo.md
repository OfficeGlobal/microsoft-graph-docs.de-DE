---
title: Ressourcentyp participantInfo
description: Enthält zusätzliche Eigenschaften über die Teilnehmerliste Identität
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7860c80da8e0f56ca425cffe8876d6003fba1d0d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991412"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="16de7-103">Ressourcentyp participantInfo</span><span class="sxs-lookup"><span data-stu-id="16de7-103">participantInfo resource type</span></span>

> <span data-ttu-id="16de7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="16de7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16de7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16de7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16de7-106">Enthält zusätzliche Eigenschaften über die Teilnehmerliste Identität</span><span class="sxs-lookup"><span data-stu-id="16de7-106">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="16de7-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="16de7-107">Properties</span></span>

| <span data-ttu-id="16de7-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="16de7-108">Property</span></span>       | <span data-ttu-id="16de7-109">Typ</span><span class="sxs-lookup"><span data-stu-id="16de7-109">Type</span></span>                          | <span data-ttu-id="16de7-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16de7-110">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="16de7-111">Identität</span><span class="sxs-lookup"><span data-stu-id="16de7-111">identity</span></span>       | [<span data-ttu-id="16de7-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="16de7-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="16de7-113">Die [IdentitySet](identityset.md) dieser Teilnehmer zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="16de7-113">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="16de7-114">languageId</span><span class="sxs-lookup"><span data-stu-id="16de7-114">languageId</span></span>     | <span data-ttu-id="16de7-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="16de7-115">String</span></span>                        | <span data-ttu-id="16de7-116">Die Sprache-Kultur-Zeichenfolge.</span><span class="sxs-lookup"><span data-stu-id="16de7-116">The language culture string.</span></span> |
| <span data-ttu-id="16de7-117">Region</span><span class="sxs-lookup"><span data-stu-id="16de7-117">region</span></span>         | <span data-ttu-id="16de7-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="16de7-118">String</span></span>                        | <span data-ttu-id="16de7-119">Region des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="16de7-119">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="16de7-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="16de7-120">JSON representation</span></span>

<span data-ttu-id="16de7-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="16de7-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId", "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "languageId": "String",
  "region": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
