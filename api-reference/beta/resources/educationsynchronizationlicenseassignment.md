---
title: Ressourcentyp educationSynchronizationLicenseAssignment
description: Stellt die Lizenzinformationen Benutzerkonten zugewiesen. Die Ressource wird Lizenz Zuordnungen einrichten, beim Erstellen von neuen Benutzerkonten verwendet werden.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c60b868ab8d973f6249d7e9ea2b30415d4b8a1b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409678"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="826f4-104">Ressourcentyp educationSynchronizationLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="826f4-104">educationSynchronizationLicenseAssignment resource type</span></span>

> <span data-ttu-id="826f4-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="826f4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="826f4-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="826f4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="826f4-107">Stellt die Lizenzinformationen Benutzerkonten zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="826f4-107">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="826f4-108">Die Ressource wird Lizenz Zuordnungen einrichten, beim Erstellen von neuen Benutzerkonten verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="826f4-108">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="826f4-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="826f4-109">Properties</span></span>

| <span data-ttu-id="826f4-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="826f4-110">Property</span></span> | <span data-ttu-id="826f4-111">Typ</span><span class="sxs-lookup"><span data-stu-id="826f4-111">Type</span></span> | <span data-ttu-id="826f4-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="826f4-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="826f4-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="826f4-113">**appliesTo**</span></span> | <span data-ttu-id="826f4-114">string</span><span class="sxs-lookup"><span data-stu-id="826f4-114">string</span></span> | <span data-ttu-id="826f4-115">Der Benutzer Rollentyp Lizenz zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="826f4-115">The user role type to assign to license.</span></span> <span data-ttu-id="826f4-116">Mögliche Werte sind: `student` und `teacher`.</span><span class="sxs-lookup"><span data-stu-id="826f4-116">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="826f4-117">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="826f4-117">**skuIds**</span></span> | <span data-ttu-id="826f4-118">Auflistung von Zeichenfolgen</span><span class="sxs-lookup"><span data-stu-id="826f4-118">collection of strings</span></span> |  <span data-ttu-id="826f4-119">Stellt die SKU-Bezeichner, der die Lizenzen zuweisen.</span><span class="sxs-lookup"><span data-stu-id="826f4-119">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="826f4-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="826f4-120">JSON representation</span></span>
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
