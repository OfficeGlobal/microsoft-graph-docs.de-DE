---
title: domainState-Ressourcentyp
description: Stellt den Status asynchroner Vorgänge dar, die in einer Domäne geplant sind.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6a7741448b9c91be32f67f89cbafa5a579320083
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938293"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="5515a-103">domainState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5515a-103">domainState resource type</span></span>

<span data-ttu-id="5515a-104">Stellt den Status asynchroner Vorgänge dar, die in einer Domäne geplant sind.</span><span class="sxs-lookup"><span data-stu-id="5515a-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="5515a-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5515a-105">Properties</span></span>

| <span data-ttu-id="5515a-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5515a-106">Property</span></span>   | <span data-ttu-id="5515a-107">Typ</span><span class="sxs-lookup"><span data-stu-id="5515a-107">Type</span></span> | <span data-ttu-id="5515a-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5515a-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="5515a-109">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="5515a-109">lastActionDateTime</span></span> | <span data-ttu-id="5515a-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5515a-110">DateTimeOffset</span></span> | <span data-ttu-id="5515a-p101">Zeitstempel der letzten Aktivität. Der Wert wird aktualisiert, wenn ein Vorgang geplant, die asynchrone Aufgabe gestartet und der Vorgang abgeschlossen wird.</span><span class="sxs-lookup"><span data-stu-id="5515a-p101">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="5515a-113">Operation</span><span class="sxs-lookup"><span data-stu-id="5515a-113">operation</span></span> | <span data-ttu-id="5515a-114">String</span><span class="sxs-lookup"><span data-stu-id="5515a-114">String</span></span> | <span data-ttu-id="5515a-p102">Typ des asynchronen Vorgangs. Mögliche Werte sind *ForceDelete* und *Verification*</span><span class="sxs-lookup"><span data-stu-id="5515a-p102">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="5515a-117">status</span><span class="sxs-lookup"><span data-stu-id="5515a-117">status</span></span> | <span data-ttu-id="5515a-118">String</span><span class="sxs-lookup"><span data-stu-id="5515a-118">String</span></span> | <span data-ttu-id="5515a-119">Der aktuellen Status des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="5515a-119">Current status of the operation.</span></span> <br> <span data-ttu-id="5515a-120">*Scheduled*: Der Vorgang wurde geplant, aber noch nicht gestartet.</span><span class="sxs-lookup"><span data-stu-id="5515a-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="5515a-121">*InProgress*: Der Vorgang wurde gestartet und wird ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="5515a-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="5515a-122">*Failed*: Ein Fehler ist im Vorgang aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="5515a-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5515a-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5515a-123">JSON representation</span></span>
<span data-ttu-id="5515a-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5515a-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
