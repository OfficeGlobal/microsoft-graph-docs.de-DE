---
title: Ressourcentyp teamsTemplate
description: Beschreibt die TeamsTemplate Entität.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e75b3d8df318b116d5d908a40d4f756d9ee70864
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513046"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="ba450-103">Ressourcentyp teamsTemplate</span><span class="sxs-lookup"><span data-stu-id="ba450-103">teamsTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba450-104">Eine Teamvorlage ist eine Vorlage für ein [Team](../resources/team.md) in Microsoft-Teams erstellen.</span><span class="sxs-lookup"><span data-stu-id="ba450-104">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="ba450-105">Eine Vorlage gibt die Struktur, Einstellungen und sogar Inhalte, die bereitgestellt werden soll in ein neues Team mit der Vorlage erstellt.</span><span class="sxs-lookup"><span data-stu-id="ba450-105">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="ba450-106">Microsoft bietet eine Reihe von Basis Vorlagen und Kunden können ihre eigenen benutzerdefinierten Vorlagen gespeichert.</span><span class="sxs-lookup"><span data-stu-id="ba450-106">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="ba450-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ba450-107">Properties</span></span>

| <span data-ttu-id="ba450-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ba450-108">Property</span></span>            | <span data-ttu-id="ba450-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ba450-109">Type</span></span>     | <span data-ttu-id="ba450-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ba450-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="ba450-111">id</span><span class="sxs-lookup"><span data-stu-id="ba450-111">id</span></span>                  | <span data-ttu-id="ba450-112">String</span><span class="sxs-lookup"><span data-stu-id="ba450-112">String</span></span>   | <span data-ttu-id="ba450-113">Eindeutiger Bezeichner der Vorlage.</span><span class="sxs-lookup"><span data-stu-id="ba450-113">Unique identifier of the template.</span></span> <span data-ttu-id="ba450-114">Darf nicht null sein.</span><span class="sxs-lookup"><span data-stu-id="ba450-114">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ba450-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ba450-115">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a><span data-ttu-id="ba450-116">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="ba450-116">See also</span></span>

- <span data-ttu-id="ba450-117">Team</span><span class="sxs-lookup"><span data-stu-id="ba450-117">[team](team.md)</span></span>

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
