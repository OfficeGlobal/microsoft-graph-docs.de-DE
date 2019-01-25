---
title: Ressourcentyp educationSynchronizationLicenseAssignment
description: Stellt die Lizenzinformationen Benutzerkonten zugewiesen. Die Ressource wird Lizenz Zuordnungen einrichten, beim Erstellen von neuen Benutzerkonten verwendet werden.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ce1ae196ba4f014a039e81713119b01fa69e6170
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525822"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="90ff5-104">Ressourcentyp educationSynchronizationLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="90ff5-104">educationSynchronizationLicenseAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90ff5-105">Stellt die Lizenzinformationen Benutzerkonten zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="90ff5-105">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="90ff5-106">Die Ressource wird Lizenz Zuordnungen einrichten, beim Erstellen von neuen Benutzerkonten verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="90ff5-106">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="90ff5-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="90ff5-107">Properties</span></span>

| <span data-ttu-id="90ff5-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="90ff5-108">Property</span></span> | <span data-ttu-id="90ff5-109">Typ</span><span class="sxs-lookup"><span data-stu-id="90ff5-109">Type</span></span> | <span data-ttu-id="90ff5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90ff5-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="90ff5-111">appliesTo</span><span class="sxs-lookup"><span data-stu-id="90ff5-111">**appliesTo**</span></span> | <span data-ttu-id="90ff5-112">string</span><span class="sxs-lookup"><span data-stu-id="90ff5-112">string</span></span> | <span data-ttu-id="90ff5-113">Der Benutzer Rollentyp Lizenz zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="90ff5-113">The user role type to assign to license.</span></span> <span data-ttu-id="90ff5-114">Mögliche Werte sind: `student` und `teacher`.</span><span class="sxs-lookup"><span data-stu-id="90ff5-114">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="90ff5-115">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="90ff5-115">**skuIds**</span></span> | <span data-ttu-id="90ff5-116">Auflistung von Zeichenfolgen</span><span class="sxs-lookup"><span data-stu-id="90ff5-116">collection of strings</span></span> |  <span data-ttu-id="90ff5-117">Stellt die SKU-Bezeichner, der die Lizenzen zuweisen.</span><span class="sxs-lookup"><span data-stu-id="90ff5-117">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="90ff5-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="90ff5-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationlicenseassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
