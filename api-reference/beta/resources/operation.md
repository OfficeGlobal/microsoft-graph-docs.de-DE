---
title: Vorgang Ressourcentyp
description: Der Status der ein zeitintensiver Vorgang.
localization_priority: Normal
ms.openlocfilehash: 3ad9848387dab2de928f7ace2fa4b905720be615
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520186"
---
# <a name="operation-resource-type"></a><span data-ttu-id="3ef16-103">Vorgang Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3ef16-103">operation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ef16-104">Der Status der ein zeitintensiver Vorgang.</span><span class="sxs-lookup"><span data-stu-id="3ef16-104">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="3ef16-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="3ef16-105">Methods</span></span>

<span data-ttu-id="3ef16-106">Keine</span><span class="sxs-lookup"><span data-stu-id="3ef16-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="3ef16-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3ef16-107">Properties</span></span>

| <span data-ttu-id="3ef16-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3ef16-108">Property</span></span>           | <span data-ttu-id="3ef16-109">Typ</span><span class="sxs-lookup"><span data-stu-id="3ef16-109">Type</span></span>            | <span data-ttu-id="3ef16-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ef16-110">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="3ef16-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ef16-111">createdDateTime</span></span>    | <span data-ttu-id="3ef16-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ef16-112">DateTimeOffset</span></span>  | <span data-ttu-id="3ef16-113">Die Startzeit des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="3ef16-113">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="3ef16-114">id</span><span class="sxs-lookup"><span data-stu-id="3ef16-114">id</span></span>                 | <span data-ttu-id="3ef16-115">String</span><span class="sxs-lookup"><span data-stu-id="3ef16-115">String</span></span>          | <span data-ttu-id="3ef16-116">Die Vorgangs-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3ef16-116">The operation id. Read-only.</span></span> <span data-ttu-id="3ef16-117">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="3ef16-117">Server generated.</span></span>                                  |
| <span data-ttu-id="3ef16-118">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="3ef16-118">lastActionDateTime</span></span> | <span data-ttu-id="3ef16-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ef16-119">DateTimeOffset</span></span>  | <span data-ttu-id="3ef16-120">Der Zeitpunkt der letzten Aktion des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="3ef16-120">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="3ef16-121">status</span><span class="sxs-lookup"><span data-stu-id="3ef16-121">status</span></span>             | <span data-ttu-id="3ef16-122">String</span><span class="sxs-lookup"><span data-stu-id="3ef16-122">String</span></span>          | <span data-ttu-id="3ef16-123">Mögliche Werte: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="3ef16-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="3ef16-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3ef16-124">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3ef16-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3ef16-125">Relationships</span></span>

<span data-ttu-id="3ef16-126">Keine</span><span class="sxs-lookup"><span data-stu-id="3ef16-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ef16-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3ef16-127">JSON representation</span></span>

<span data-ttu-id="3ef16-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3ef16-128">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="3ef16-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3ef16-129">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "status": "completed"
}
```

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/operation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
