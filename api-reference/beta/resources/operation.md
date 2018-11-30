---
title: Vorgang Ressourcentyp
description: Der Status der ein zeitintensiver Vorgang.
ms.openlocfilehash: 71e6a1c47e1f3b18f1481700320779714d716bec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060834"
---
# <a name="operation-resource-type"></a><span data-ttu-id="7e51c-103">Vorgang Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7e51c-103">operation resource type</span></span>

> <span data-ttu-id="7e51c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7e51c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e51c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7e51c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7e51c-106">Der Status der ein zeitintensiver Vorgang.</span><span class="sxs-lookup"><span data-stu-id="7e51c-106">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="7e51c-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="7e51c-107">Methods</span></span>

<span data-ttu-id="7e51c-108">Keine</span><span class="sxs-lookup"><span data-stu-id="7e51c-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="7e51c-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7e51c-109">Properties</span></span>

| <span data-ttu-id="7e51c-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7e51c-110">Property</span></span>           | <span data-ttu-id="7e51c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="7e51c-111">Type</span></span>            | <span data-ttu-id="7e51c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e51c-112">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="7e51c-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e51c-113">createdDateTime</span></span>    | <span data-ttu-id="7e51c-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e51c-114">DateTimeOffset</span></span>  | <span data-ttu-id="7e51c-115">Die Startzeit des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="7e51c-115">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="7e51c-116">id</span><span class="sxs-lookup"><span data-stu-id="7e51c-116">id</span></span>                 | <span data-ttu-id="7e51c-117">String</span><span class="sxs-lookup"><span data-stu-id="7e51c-117">String</span></span>          | <span data-ttu-id="7e51c-118">Die Vorgangs-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7e51c-118">The operation id. Read-only.</span></span> <span data-ttu-id="7e51c-119">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="7e51c-119">Server generated.</span></span>                                  |
| <span data-ttu-id="7e51c-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="7e51c-120">lastActionDateTime</span></span> | <span data-ttu-id="7e51c-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e51c-121">DateTimeOffset</span></span>  | <span data-ttu-id="7e51c-122">Der Zeitpunkt der letzten Aktion des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="7e51c-122">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="7e51c-123">status</span><span class="sxs-lookup"><span data-stu-id="7e51c-123">status</span></span>             | <span data-ttu-id="7e51c-124">String</span><span class="sxs-lookup"><span data-stu-id="7e51c-124">String</span></span>          | <span data-ttu-id="7e51c-125">Mögliche Werte: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="7e51c-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="7e51c-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7e51c-126">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7e51c-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7e51c-127">Relationships</span></span>

<span data-ttu-id="7e51c-128">Keine</span><span class="sxs-lookup"><span data-stu-id="7e51c-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e51c-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7e51c-129">JSON representation</span></span>

<span data-ttu-id="7e51c-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7e51c-130">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="7e51c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7e51c-131">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->