---
title: educationTeacher-Ressourcentyp
description: Zusätzliche Informationen, die einem vorhandenen educationUser hinzugefügt werden, wenn die primaryRole eines Benutzers `teacher` ist.
ms.openlocfilehash: 37fd46ee00f82b518d91969b1793147be859efdf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058139"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="1b9b9-103">educationTeacher-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1b9b9-103">educationTeacher resource type</span></span>

> <span data-ttu-id="1b9b9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1b9b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b9b9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1b9b9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1b9b9-106">Zusätzliche Informationen, die einem vorhandenen [educationUser](educationuser.md) hinzugefügt werden, wenn die primaryRole eines Benutzers `teacher` ist.</span><span class="sxs-lookup"><span data-stu-id="1b9b9-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="1b9b9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1b9b9-107">Properties</span></span>
| <span data-ttu-id="1b9b9-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1b9b9-108">Property</span></span>     | <span data-ttu-id="1b9b9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="1b9b9-109">Type</span></span>   |<span data-ttu-id="1b9b9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b9b9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b9b9-111">externalId</span><span class="sxs-lookup"><span data-stu-id="1b9b9-111">externalId</span></span>|<span data-ttu-id="1b9b9-112">String</span><span class="sxs-lookup"><span data-stu-id="1b9b9-112">String</span></span>| <span data-ttu-id="1b9b9-113">Die ID der Lehrkraft im Quellsystem.</span><span class="sxs-lookup"><span data-stu-id="1b9b9-113">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="1b9b9-114">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="1b9b9-114">teacherNumber</span></span>|<span data-ttu-id="1b9b9-115">String</span><span class="sxs-lookup"><span data-stu-id="1b9b9-115">String</span></span>|<span data-ttu-id="1b9b9-116">Lehrernummer</span><span class="sxs-lookup"><span data-stu-id="1b9b9-116">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b9b9-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1b9b9-117">JSON representation</span></span>

<span data-ttu-id="1b9b9-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1b9b9-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeacher"
}-->

```json
{
  "externalId": "String",
  "teacherNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->