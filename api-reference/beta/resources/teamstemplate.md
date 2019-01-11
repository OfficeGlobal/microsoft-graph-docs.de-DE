---
title: Ressourcentyp teamsTemplate
description: Beschreibt die TeamsTemplate Entität.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 6e847c7ef0b13dd9c4281c17939164128be8b6a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818872"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="6890f-103">Ressourcentyp teamsTemplate</span><span class="sxs-lookup"><span data-stu-id="6890f-103">teamsTemplate resource type</span></span>

> <span data-ttu-id="6890f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6890f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6890f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6890f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6890f-106">Eine Teamvorlage ist eine Vorlage für ein [Team](../resources/team.md) in Microsoft-Teams erstellen.</span><span class="sxs-lookup"><span data-stu-id="6890f-106">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="6890f-107">Eine Vorlage gibt die Struktur, Einstellungen und sogar Inhalte, die bereitgestellt werden soll in ein neues Team mit der Vorlage erstellt.</span><span class="sxs-lookup"><span data-stu-id="6890f-107">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="6890f-108">Microsoft bietet eine Reihe von Basis Vorlagen und Kunden können ihre eigenen benutzerdefinierten Vorlagen gespeichert.</span><span class="sxs-lookup"><span data-stu-id="6890f-108">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="6890f-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6890f-109">Properties</span></span>

| <span data-ttu-id="6890f-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6890f-110">Property</span></span>            | <span data-ttu-id="6890f-111">Typ</span><span class="sxs-lookup"><span data-stu-id="6890f-111">Type</span></span>     | <span data-ttu-id="6890f-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6890f-112">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="6890f-113">id</span><span class="sxs-lookup"><span data-stu-id="6890f-113">id</span></span>                  | <span data-ttu-id="6890f-114">String</span><span class="sxs-lookup"><span data-stu-id="6890f-114">String</span></span>   | <span data-ttu-id="6890f-115">Eindeutiger Bezeichner der Vorlage.</span><span class="sxs-lookup"><span data-stu-id="6890f-115">Unique identifier of the template.</span></span> <span data-ttu-id="6890f-116">Darf nicht null sein.</span><span class="sxs-lookup"><span data-stu-id="6890f-116">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6890f-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6890f-117">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="6890f-118">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="6890f-118">See also</span></span>

- [<span data-ttu-id="6890f-119">Team</span><span class="sxs-lookup"><span data-stu-id="6890f-119">team</span></span>](team.md)

