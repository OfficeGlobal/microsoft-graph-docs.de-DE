---
title: Ressourcentyp educationSubmissionIndividualRecipient
description: 'Eine Unterklasse der EducationSubmissionRecipient, der angibt, dass eine Übermittlung an eine Person in der Klasse zugewiesen ist.  '
ms.openlocfilehash: 4b74defc1a21427b6169e399262d827561178e5f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058855"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a><span data-ttu-id="bab5c-103">Ressourcentyp educationSubmissionIndividualRecipient</span><span class="sxs-lookup"><span data-stu-id="bab5c-103">educationSubmissionIndividualRecipient resource type</span></span>

> <span data-ttu-id="bab5c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bab5c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bab5c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bab5c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bab5c-106">Eine Unterklasse der [EducationSubmissionRecipient](educationsubmissionrecipient.md) , der angibt, dass eine Übermittlung an eine Person in der Klasse zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="bab5c-106">A subclass of [educationSubmissionRecipient](educationsubmissionrecipient.md) that indicates that a submission is assigned to an individual in the class.</span></span>  


## <a name="properties"></a><span data-ttu-id="bab5c-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bab5c-107">Properties</span></span>
| <span data-ttu-id="bab5c-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bab5c-108">Property</span></span>     | <span data-ttu-id="bab5c-109">Typ</span><span class="sxs-lookup"><span data-stu-id="bab5c-109">Type</span></span>   |<span data-ttu-id="bab5c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bab5c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bab5c-111">userId</span><span class="sxs-lookup"><span data-stu-id="bab5c-111">userId</span></span>|<span data-ttu-id="bab5c-112">String</span><span class="sxs-lookup"><span data-stu-id="bab5c-112">String</span></span>|<span data-ttu-id="bab5c-113">Benutzer-ID des Benutzers, dem die Übermittlung zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="bab5c-113">User ID of the user to whom the submission is assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bab5c-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bab5c-114">JSON representation</span></span>

<span data-ttu-id="bab5c-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bab5c-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionIndividualRecipient"
}-->

```json
{
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmissionIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->