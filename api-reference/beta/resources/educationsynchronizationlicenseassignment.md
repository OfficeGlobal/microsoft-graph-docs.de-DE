---
title: Ressourcentyp educationSynchronizationLicenseAssignment
description: Stellt die Lizenzinformationen Benutzerkonten zugewiesen. Die Ressource wird Lizenz Zuordnungen einrichten, beim Erstellen von neuen Benutzerkonten verwendet werden.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 757e080a8b2c6f3f01fa1663f10c9b0b98eaf4d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948275"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="3e1a2-104">Ressourcentyp educationSynchronizationLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="3e1a2-104">educationSynchronizationLicenseAssignment resource type</span></span>

> <span data-ttu-id="3e1a2-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3e1a2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e1a2-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3e1a2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e1a2-107">Stellt die Lizenzinformationen Benutzerkonten zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="3e1a2-107">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="3e1a2-108">Die Ressource wird Lizenz Zuordnungen einrichten, beim Erstellen von neuen Benutzerkonten verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="3e1a2-108">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="3e1a2-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3e1a2-109">Properties</span></span>

| <span data-ttu-id="3e1a2-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3e1a2-110">Property</span></span> | <span data-ttu-id="3e1a2-111">Typ</span><span class="sxs-lookup"><span data-stu-id="3e1a2-111">Type</span></span> | <span data-ttu-id="3e1a2-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e1a2-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="3e1a2-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="3e1a2-113">**appliesTo**</span></span> | <span data-ttu-id="3e1a2-114">string</span><span class="sxs-lookup"><span data-stu-id="3e1a2-114">string</span></span> | <span data-ttu-id="3e1a2-115">Der Benutzer Rollentyp Lizenz zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="3e1a2-115">The user role type to assign to license.</span></span> <span data-ttu-id="3e1a2-116">Mögliche Werte sind: `student` und `teacher`.</span><span class="sxs-lookup"><span data-stu-id="3e1a2-116">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="3e1a2-117">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="3e1a2-117">**skuIds**</span></span> | <span data-ttu-id="3e1a2-118">Auflistung von Zeichenfolgen</span><span class="sxs-lookup"><span data-stu-id="3e1a2-118">collection of strings</span></span> |  <span data-ttu-id="3e1a2-119">Stellt die SKU-Bezeichner, der die Lizenzen zuweisen.</span><span class="sxs-lookup"><span data-stu-id="3e1a2-119">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="3e1a2-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3e1a2-120">JSON representation</span></span>
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
