---
title: Ressourcentyp freeBusyError
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 63cfc4b14ba6176d582155df57b7f7f787e63cf4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889768"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="9bbd7-104">Ressourcentyp freeBusyError</span><span class="sxs-lookup"><span data-stu-id="9bbd7-104">freeBusyError resource type</span></span>

 > <span data-ttu-id="9bbd7-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9bbd7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bbd7-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9bbd7-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="9bbd7-107">Stellt Informationen zum Fehler versucht, die die Verfügbarkeit von einem Benutzer, eine Verteilerliste oder eine Ressource erhalten möchten.</span><span class="sxs-lookup"><span data-stu-id="9bbd7-107">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="9bbd7-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9bbd7-108">Properties</span></span>
| <span data-ttu-id="9bbd7-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9bbd7-109">Property</span></span>     | <span data-ttu-id="9bbd7-110">Typ</span><span class="sxs-lookup"><span data-stu-id="9bbd7-110">Type</span></span>   |<span data-ttu-id="9bbd7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9bbd7-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9bbd7-112">message</span><span class="sxs-lookup"><span data-stu-id="9bbd7-112">message</span></span> |<span data-ttu-id="9bbd7-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9bbd7-113">String</span></span> |<span data-ttu-id="9bbd7-114">Beschreibt den Fehler.</span><span class="sxs-lookup"><span data-stu-id="9bbd7-114">Describes the error.</span></span> |
|<span data-ttu-id="9bbd7-115">responseCode</span><span class="sxs-lookup"><span data-stu-id="9bbd7-115">responseCode</span></span> |<span data-ttu-id="9bbd7-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9bbd7-116">String</span></span> |<span data-ttu-id="9bbd7-117">Der Antwortcode von Abfragen für die Verfügbarkeit des Benutzers, der Verteilerliste oder der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9bbd7-117">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="9bbd7-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9bbd7-118">JSON representation</span></span>

<span data-ttu-id="9bbd7-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9bbd7-119">The following is a JSON representation of the resource.</span></span>

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
