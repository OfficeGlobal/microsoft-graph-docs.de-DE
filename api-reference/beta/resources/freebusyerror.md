---
title: freeBusyError-Ressourcentyp
description: Stellt Fehlerinformationen aus dem Versuch, die Verfügbarkeit eines Benutzers, einer Verteilerliste oder einer Ressource zu erhalten.
localization_priority: Normal
ms.openlocfilehash: e2c755b51e72adf3ff4efa4de5c9438e70d701e1
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869337"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="7225e-103">freeBusyError-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7225e-103">freeBusyError resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="7225e-104">Stellt Fehlerinformationen aus dem Versuch, die Verfügbarkeit eines Benutzers, einer Verteilerliste oder einer Ressource zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="7225e-104">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="7225e-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7225e-105">Properties</span></span>
| <span data-ttu-id="7225e-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7225e-106">Property</span></span>     | <span data-ttu-id="7225e-107">Typ</span><span class="sxs-lookup"><span data-stu-id="7225e-107">Type</span></span>   |<span data-ttu-id="7225e-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7225e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7225e-109">message</span><span class="sxs-lookup"><span data-stu-id="7225e-109">message</span></span> |<span data-ttu-id="7225e-110">String</span><span class="sxs-lookup"><span data-stu-id="7225e-110">String</span></span> |<span data-ttu-id="7225e-111">Beschreibt den Fehler.</span><span class="sxs-lookup"><span data-stu-id="7225e-111">Describes the error.</span></span> |
|<span data-ttu-id="7225e-112">Response Code</span><span class="sxs-lookup"><span data-stu-id="7225e-112">responseCode</span></span> |<span data-ttu-id="7225e-113">String</span><span class="sxs-lookup"><span data-stu-id="7225e-113">String</span></span> |<span data-ttu-id="7225e-114">Der Antwortcode aus der Abfrage für die Verfügbarkeit des Benutzers, der Verteilerliste oder der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7225e-114">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="7225e-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7225e-115">JSON representation</span></span>

<span data-ttu-id="7225e-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7225e-116">The following is a JSON representation of the resource.</span></span>

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
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/freebusyerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
