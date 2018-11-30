---
title: Ressourcentyp educationSynchronizationLicenseAssignment
description: Stellt die Lizenzinformationen Benutzerkonten zugewiesen. Die Ressource wird Lizenz Zuordnungen einrichten, beim Erstellen von neuen Benutzerkonten verwendet werden.
ms.openlocfilehash: a324007dc4d6b5557db407c39d27a640f56ceb55
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064021"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="017fe-104">Ressourcentyp educationSynchronizationLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="017fe-104">educationSynchronizationLicenseAssignment resource type</span></span>

> <span data-ttu-id="017fe-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="017fe-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="017fe-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="017fe-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="017fe-107">Stellt die Lizenzinformationen Benutzerkonten zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="017fe-107">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="017fe-108">Die Ressource wird Lizenz Zuordnungen einrichten, beim Erstellen von neuen Benutzerkonten verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="017fe-108">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="017fe-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="017fe-109">Properties</span></span>

| <span data-ttu-id="017fe-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="017fe-110">Property</span></span> | <span data-ttu-id="017fe-111">Typ</span><span class="sxs-lookup"><span data-stu-id="017fe-111">Type</span></span> | <span data-ttu-id="017fe-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="017fe-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="017fe-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="017fe-113">**appliesTo**</span></span> | <span data-ttu-id="017fe-114">string</span><span class="sxs-lookup"><span data-stu-id="017fe-114">string</span></span> | <span data-ttu-id="017fe-115">Der Benutzer Rollentyp Lizenz zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="017fe-115">The user role type to assign to license.</span></span> <span data-ttu-id="017fe-116">Mögliche Werte sind: `student` und `teacher`.</span><span class="sxs-lookup"><span data-stu-id="017fe-116">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="017fe-117">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="017fe-117">**skuIds**</span></span> | <span data-ttu-id="017fe-118">Auflistung von Zeichenfolgen</span><span class="sxs-lookup"><span data-stu-id="017fe-118">collection of strings</span></span> |  <span data-ttu-id="017fe-119">Stellt die SKU-Bezeichner, der die Lizenzen zuweisen.</span><span class="sxs-lookup"><span data-stu-id="017fe-119">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="017fe-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="017fe-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
