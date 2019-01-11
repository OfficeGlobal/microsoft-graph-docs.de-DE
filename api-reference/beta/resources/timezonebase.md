---
title: timeZoneBase-Ressourcentyp
description: Die grundlegende Darstellung einer Zeitzone.
localization_priority: Normal
ms.openlocfilehash: 95d3409c40b3cc151f7b2f4b69580b9c1bbbe1ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882453"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="d1c52-103">timeZoneBase-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d1c52-103">timeZoneBase resource type</span></span>

> <span data-ttu-id="d1c52-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d1c52-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1c52-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d1c52-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1c52-106">Die grundlegende Darstellung einer Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="d1c52-106">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="d1c52-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d1c52-107">Properties</span></span>
| <span data-ttu-id="d1c52-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d1c52-108">Property</span></span>     | <span data-ttu-id="d1c52-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d1c52-109">Type</span></span>   |<span data-ttu-id="d1c52-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1c52-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d1c52-111">name</span><span class="sxs-lookup"><span data-stu-id="d1c52-111">name</span></span> | <span data-ttu-id="d1c52-112">string</span><span class="sxs-lookup"><span data-stu-id="d1c52-112">string</span></span> | <span data-ttu-id="d1c52-113">Der Name einer Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="d1c52-113">The name of a time zone.</span></span> <span data-ttu-id="d1c52-114">Dies kann ein standardmäßiger Name für eine Zeitzone sein, z. B. „Hawaii-Aleutian Normalzeit“ oder „Benutzerdefinierte Zeitzone“ für eine benutzerdefinierte Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="d1c52-114">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="d1c52-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d1c52-115">JSON representation</span></span>

<span data-ttu-id="d1c52-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d1c52-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
