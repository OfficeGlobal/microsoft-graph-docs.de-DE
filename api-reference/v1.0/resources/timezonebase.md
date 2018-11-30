---
title: timeZoneBase-Ressourcentyp
description: Die grundlegende Darstellung einer Zeitzone.
ms.openlocfilehash: 18df657ab561163b64bcf224f8902f2ba7e0039c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018109"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="26d28-103">timeZoneBase-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="26d28-103">timeZoneBase resource type</span></span>

<span data-ttu-id="26d28-104">Die grundlegende Darstellung einer Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="26d28-104">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="26d28-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="26d28-105">Properties</span></span>
| <span data-ttu-id="26d28-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="26d28-106">Property</span></span>     | <span data-ttu-id="26d28-107">Typ</span><span class="sxs-lookup"><span data-stu-id="26d28-107">Type</span></span>   |<span data-ttu-id="26d28-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26d28-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="26d28-109">name</span><span class="sxs-lookup"><span data-stu-id="26d28-109">name</span></span> | <span data-ttu-id="26d28-110">string</span><span class="sxs-lookup"><span data-stu-id="26d28-110">string</span></span> | <span data-ttu-id="26d28-111">Der Name einer Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="26d28-111">The name of a time zone.</span></span> <span data-ttu-id="26d28-112">Dies kann ein standardmäßiger Name für eine Zeitzone sein, z. B. „Hawaii-Aleutian Normalzeit“ oder „Benutzerdefinierte Zeitzone“ für eine benutzerdefinierte Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="26d28-112">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="26d28-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="26d28-113">JSON representation</span></span>

<span data-ttu-id="26d28-114">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="26d28-114">Here is a JSON representation of the resource.</span></span>

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