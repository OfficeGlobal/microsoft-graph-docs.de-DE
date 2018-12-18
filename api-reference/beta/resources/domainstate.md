---
title: domainState-Ressourcentyp
description: Stellt den Status asynchroner Vorgänge dar, die in einer Domäne geplant sind.
author: lleonard-msft
ms.openlocfilehash: 683390998254cbf3f7146d1fe89a0a2f109be320
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355888"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="3c867-103">domainState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3c867-103">domainState resource type</span></span>

> <span data-ttu-id="3c867-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3c867-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c867-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c867-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c867-106">Stellt den Status asynchroner Vorgänge dar, die in einer Domäne geplant sind.</span><span class="sxs-lookup"><span data-stu-id="3c867-106">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="3c867-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3c867-107">Properties</span></span>

| <span data-ttu-id="3c867-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3c867-108">Property</span></span>   | <span data-ttu-id="3c867-109">Typ</span><span class="sxs-lookup"><span data-stu-id="3c867-109">Type</span></span> | <span data-ttu-id="3c867-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c867-110">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="3c867-111">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="3c867-111">lastActionDateTime</span></span> | <span data-ttu-id="3c867-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c867-112">DateTimeOffset</span></span> | <span data-ttu-id="3c867-p102">Zeitstempel der letzten Aktivität. Der Wert wird aktualisiert, wenn ein Vorgang geplant, die asynchrone Aufgabe gestartet und der Vorgang abgeschlossen wird.</span><span class="sxs-lookup"><span data-stu-id="3c867-p102">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="3c867-115">Operation</span><span class="sxs-lookup"><span data-stu-id="3c867-115">operation</span></span> | <span data-ttu-id="3c867-116">String</span><span class="sxs-lookup"><span data-stu-id="3c867-116">String</span></span> | <span data-ttu-id="3c867-p103">Typ des asynchronen Vorgangs. Mögliche Werte sind *ForceDelete* und *Verification*</span><span class="sxs-lookup"><span data-stu-id="3c867-p103">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="3c867-119">status</span><span class="sxs-lookup"><span data-stu-id="3c867-119">status</span></span> | <span data-ttu-id="3c867-120">String</span><span class="sxs-lookup"><span data-stu-id="3c867-120">String</span></span> | <span data-ttu-id="3c867-121">Der aktuellen Status des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="3c867-121">Current status of the operation.</span></span> <br> <span data-ttu-id="3c867-122">*Scheduled*: Der Vorgang wurde geplant, aber noch nicht gestartet.</span><span class="sxs-lookup"><span data-stu-id="3c867-122">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="3c867-123">*InProgress*: Der Vorgang wurde gestartet und wird ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="3c867-123">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="3c867-124">*Failed*: Ein Fehler ist im Vorgang aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="3c867-124">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3c867-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3c867-125">JSON representation</span></span>
<span data-ttu-id="3c867-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3c867-126">Here is a JSON representation of the resource.</span></span>

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