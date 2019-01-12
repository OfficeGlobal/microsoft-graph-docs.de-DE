---
title: Ressourcentyp teamsTemplate
description: Beschreibt die TeamsTemplate Entität.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9bd5047950ed1ed3c57950d2c4b708a78b570649
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940085"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="76342-103">Ressourcentyp teamsTemplate</span><span class="sxs-lookup"><span data-stu-id="76342-103">teamsTemplate resource type</span></span>

> <span data-ttu-id="76342-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="76342-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76342-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="76342-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76342-106">Eine Teamvorlage ist eine Vorlage für ein [Team](../resources/team.md) in Microsoft-Teams erstellen.</span><span class="sxs-lookup"><span data-stu-id="76342-106">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="76342-107">Eine Vorlage gibt die Struktur, Einstellungen und sogar Inhalte, die bereitgestellt werden soll in ein neues Team mit der Vorlage erstellt.</span><span class="sxs-lookup"><span data-stu-id="76342-107">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="76342-108">Microsoft bietet eine Reihe von Basis Vorlagen und Kunden können ihre eigenen benutzerdefinierten Vorlagen gespeichert.</span><span class="sxs-lookup"><span data-stu-id="76342-108">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="76342-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="76342-109">Properties</span></span>

| <span data-ttu-id="76342-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="76342-110">Property</span></span>            | <span data-ttu-id="76342-111">Typ</span><span class="sxs-lookup"><span data-stu-id="76342-111">Type</span></span>     | <span data-ttu-id="76342-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76342-112">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="76342-113">id</span><span class="sxs-lookup"><span data-stu-id="76342-113">id</span></span>                  | <span data-ttu-id="76342-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76342-114">String</span></span>   | <span data-ttu-id="76342-115">Eindeutiger Bezeichner der Vorlage.</span><span class="sxs-lookup"><span data-stu-id="76342-115">Unique identifier of the template.</span></span> <span data-ttu-id="76342-116">Darf nicht null sein.</span><span class="sxs-lookup"><span data-stu-id="76342-116">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="76342-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="76342-117">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="76342-118">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="76342-118">See also</span></span>

- [<span data-ttu-id="76342-119">Team</span><span class="sxs-lookup"><span data-stu-id="76342-119">team</span></span>](team.md)

