---
title: Ressourcentyp personDataSource
description: Stellt die Quellen, die die Benutzerdaten, beispielsweise Directory und Outlook-Kontakte stammen.
ms.openlocfilehash: 1c5aeb2cbb36398eb3c7184550235fc7194f5e1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060321"
---
# <a name="persondatasource-resource-type"></a><span data-ttu-id="5924a-103">Ressourcentyp personDataSource</span><span class="sxs-lookup"><span data-stu-id="5924a-103">personDataSource resource type</span></span>

> <span data-ttu-id="5924a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5924a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5924a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5924a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5924a-106">Stellt die Quellen, die die Benutzerdaten, beispielsweise Directory und Outlook-Kontakte stammen.</span><span class="sxs-lookup"><span data-stu-id="5924a-106">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5924a-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5924a-107">JSON representation</span></span>

<span data-ttu-id="5924a-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5924a-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personDataSource"
}-->

```json
{
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="5924a-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5924a-109">Properties</span></span>
| <span data-ttu-id="5924a-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5924a-110">Property</span></span>     | <span data-ttu-id="5924a-111">Typ</span><span class="sxs-lookup"><span data-stu-id="5924a-111">Type</span></span>   |<span data-ttu-id="5924a-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5924a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5924a-113">Typ</span><span class="sxs-lookup"><span data-stu-id="5924a-113">type</span></span>|<span data-ttu-id="5924a-114">String</span><span class="sxs-lookup"><span data-stu-id="5924a-114">String</span></span>|<span data-ttu-id="5924a-115">Der Typ der Datenquelle.</span><span class="sxs-lookup"><span data-stu-id="5924a-115">The type of data source.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personDataSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->