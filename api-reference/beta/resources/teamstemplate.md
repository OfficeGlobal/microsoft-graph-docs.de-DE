---
title: Ressourcentyp teamsTemplate
description: Beschreibt die TeamsTemplate Entität.
ms.openlocfilehash: 76b2921e884d38a57097789b1ba64df3309d141c
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/08/2018
ms.locfileid: "27210149"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="2e239-103">Ressourcentyp teamsTemplate</span><span class="sxs-lookup"><span data-stu-id="2e239-103">teamsTemplate resource type</span></span>

> <span data-ttu-id="2e239-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2e239-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e239-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2e239-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2e239-106">Eine Teamvorlage ist eine Vorlage für ein [Team](../resources/team.md) in Microsoft-Teams erstellen.</span><span class="sxs-lookup"><span data-stu-id="2e239-106">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="2e239-107">Eine Vorlage gibt die Struktur, Einstellungen und sogar Inhalte, die bereitgestellt werden soll in ein neues Team mit der Vorlage erstellt.</span><span class="sxs-lookup"><span data-stu-id="2e239-107">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="2e239-108">Microsoft bietet eine Reihe von Basis Vorlagen und Kunden können ihre eigenen benutzerdefinierten Vorlagen gespeichert.</span><span class="sxs-lookup"><span data-stu-id="2e239-108">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="2e239-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2e239-109">Properties</span></span>

| <span data-ttu-id="2e239-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2e239-110">Property</span></span>            | <span data-ttu-id="2e239-111">Typ</span><span class="sxs-lookup"><span data-stu-id="2e239-111">Type</span></span>     | <span data-ttu-id="2e239-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e239-112">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="2e239-113">id</span><span class="sxs-lookup"><span data-stu-id="2e239-113">id</span></span>                  | <span data-ttu-id="2e239-114">String</span><span class="sxs-lookup"><span data-stu-id="2e239-114">String</span></span>   | <span data-ttu-id="2e239-115">Eindeutiger Bezeichner der Vorlage.</span><span class="sxs-lookup"><span data-stu-id="2e239-115">Unique identifier of the template.</span></span> <span data-ttu-id="2e239-116">Darf nicht null sein.</span><span class="sxs-lookup"><span data-stu-id="2e239-116">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2e239-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2e239-117">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="2e239-118">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="2e239-118">See also</span></span>

- [<span data-ttu-id="2e239-119">Team</span><span class="sxs-lookup"><span data-stu-id="2e239-119">team</span></span>](team.md)

