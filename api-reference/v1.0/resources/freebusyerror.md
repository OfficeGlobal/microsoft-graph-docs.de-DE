---
title: freeBusyError-Ressourcentyp
description: Stellt Fehlerinformationen aus dem Versuch, die Verfügbarkeit eines Benutzers, einer Verteilerliste oder einer Ressource zu erhalten.
localization_priority: Normal
ms.openlocfilehash: a08fe8278644ab81f2c1fbe1c7d1530cab27d91b
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "30926604"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="fb0fa-103">freeBusyError-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fb0fa-103">freeBusyError resource type</span></span>

<span data-ttu-id="fb0fa-104">Stellt Fehlerinformationen aus dem Versuch, die Verfügbarkeit eines Benutzers, einer Verteilerliste oder einer Ressource zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="fb0fa-104">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="fb0fa-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fb0fa-105">Properties</span></span>
| <span data-ttu-id="fb0fa-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fb0fa-106">Property</span></span>     | <span data-ttu-id="fb0fa-107">Typ</span><span class="sxs-lookup"><span data-stu-id="fb0fa-107">Type</span></span>   |<span data-ttu-id="fb0fa-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fb0fa-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb0fa-109">message</span><span class="sxs-lookup"><span data-stu-id="fb0fa-109">message</span></span> |<span data-ttu-id="fb0fa-110">String</span><span class="sxs-lookup"><span data-stu-id="fb0fa-110">String</span></span> |<span data-ttu-id="fb0fa-111">Beschreibt den Fehler.</span><span class="sxs-lookup"><span data-stu-id="fb0fa-111">Describes the error.</span></span> |
|<span data-ttu-id="fb0fa-112">Response Code</span><span class="sxs-lookup"><span data-stu-id="fb0fa-112">responseCode</span></span> |<span data-ttu-id="fb0fa-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fb0fa-113">String</span></span> |<span data-ttu-id="fb0fa-114">Der Antwortcode aus der Abfrage für die Verfügbarkeit des Benutzers, der Verteilerliste oder der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fb0fa-114">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="fb0fa-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fb0fa-115">JSON representation</span></span>

<span data-ttu-id="fb0fa-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fb0fa-116">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
