---
title: Ressourcentyp freeBusyError
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: d1bf6671d6c506d9959fcd5abc8843c1a08c924b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064206"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="bbbbc-104">Ressourcentyp freeBusyError</span><span class="sxs-lookup"><span data-stu-id="bbbbc-104">freeBusyError resource type</span></span>

 > <span data-ttu-id="bbbbc-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bbbbc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbbbc-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bbbbc-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="bbbbc-107">Stellt Informationen zum Fehler versucht, die die Verfügbarkeit von einem Benutzer, eine Verteilerliste oder eine Ressource erhalten möchten.</span><span class="sxs-lookup"><span data-stu-id="bbbbc-107">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="bbbbc-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bbbbc-108">Properties</span></span>
| <span data-ttu-id="bbbbc-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bbbbc-109">Property</span></span>     | <span data-ttu-id="bbbbc-110">Typ</span><span class="sxs-lookup"><span data-stu-id="bbbbc-110">Type</span></span>   |<span data-ttu-id="bbbbc-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bbbbc-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbbbc-112">message</span><span class="sxs-lookup"><span data-stu-id="bbbbc-112">message</span></span> |<span data-ttu-id="bbbbc-113">String</span><span class="sxs-lookup"><span data-stu-id="bbbbc-113">String</span></span> |<span data-ttu-id="bbbbc-114">Beschreibt den Fehler.</span><span class="sxs-lookup"><span data-stu-id="bbbbc-114">Describes the error.</span></span> |
|<span data-ttu-id="bbbbc-115">responseCode</span><span class="sxs-lookup"><span data-stu-id="bbbbc-115">responseCode</span></span> |<span data-ttu-id="bbbbc-116">String</span><span class="sxs-lookup"><span data-stu-id="bbbbc-116">String</span></span> |<span data-ttu-id="bbbbc-117">Der Antwortcode von Abfragen für die Verfügbarkeit des Benutzers, der Verteilerliste oder der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bbbbc-117">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="bbbbc-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bbbbc-118">JSON representation</span></span>

<span data-ttu-id="bbbbc-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bbbbc-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.freeBusyError"
}-->

```json
{
  "message": "String",
  "responseCode": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->