---
title: Ressourcentyp office365GroupsActivityCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 4f3a5bf02f5f477ebab036fc9afa5d35a8061138
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064930"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="7aec0-103">Ressourcentyp office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="7aec0-103">office365GroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7aec0-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7aec0-104">Properties</span></span>

| <span data-ttu-id="7aec0-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7aec0-105">Property</span></span>               | <span data-ttu-id="7aec0-106">Typ</span><span class="sxs-lookup"><span data-stu-id="7aec0-106">Type</span></span>   | <span data-ttu-id="7aec0-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7aec0-107">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="7aec0-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7aec0-108">reportRefreshDate</span></span>      | <span data-ttu-id="7aec0-109">Datum</span><span class="sxs-lookup"><span data-stu-id="7aec0-109">Date</span></span>   | <span data-ttu-id="7aec0-110">Das aktuelle Datum des Inhalts.</span><span class="sxs-lookup"><span data-stu-id="7aec0-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="7aec0-111">exchangeEmailsReceived</span><span class="sxs-lookup"><span data-stu-id="7aec0-111">exchangeEmailsReceived</span></span> | <span data-ttu-id="7aec0-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7aec0-112">Int64</span></span>  | <span data-ttu-id="7aec0-113">Die Anzahl von Postfächern Gruppe empfangenen e-Mails.</span><span class="sxs-lookup"><span data-stu-id="7aec0-113">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="7aec0-114">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="7aec0-114">yammerMessagesPosted</span></span>   | <span data-ttu-id="7aec0-115">Int64</span><span class="sxs-lookup"><span data-stu-id="7aec0-115">Int64</span></span>  | <span data-ttu-id="7aec0-116">Die Anzahl von Nachrichten zu Yammer-Gruppen bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="7aec0-116">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="7aec0-117">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="7aec0-117">yammerMessagesRead</span></span>     | <span data-ttu-id="7aec0-118">Int64</span><span class="sxs-lookup"><span data-stu-id="7aec0-118">Int64</span></span>  | <span data-ttu-id="7aec0-119">Lesen Sie die Anzahl der Nachrichten in Yammer-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="7aec0-119">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="7aec0-120">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="7aec0-120">yammerMessagesLiked</span></span>    | <span data-ttu-id="7aec0-121">Int64</span><span class="sxs-lookup"><span data-stu-id="7aec0-121">Int64</span></span>  | <span data-ttu-id="7aec0-122">Die Anzahl der Nachrichten in Yammer-Gruppen gefallen.</span><span class="sxs-lookup"><span data-stu-id="7aec0-122">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="7aec0-123">reportDate</span><span class="sxs-lookup"><span data-stu-id="7aec0-123">reportDate</span></span>             | <span data-ttu-id="7aec0-124">Datum</span><span class="sxs-lookup"><span data-stu-id="7aec0-124">Date</span></span>   | <span data-ttu-id="7aec0-125">Das Datum, an dem eine Anzahl von e-Mails an eine Gruppenpostfach gesendet wurden, oder eine Anzahl von Nachrichten gesendet wurden, lesen oder in einer Gruppe Yammer gefallen</span><span class="sxs-lookup"><span data-stu-id="7aec0-125">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="7aec0-126">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7aec0-126">reportPeriod</span></span>           | <span data-ttu-id="7aec0-127">String</span><span class="sxs-lookup"><span data-stu-id="7aec0-127">String</span></span> | <span data-ttu-id="7aec0-128">Die Anzahl der Tage, die der Bericht wird behandelt.</span><span class="sxs-lookup"><span data-stu-id="7aec0-128">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="7aec0-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7aec0-129">JSON representation</span></span>

<span data-ttu-id="7aec0-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7aec0-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeEmailsReceived": 1024, 
  "yammerMessagesPosted": 1024, 
  "yammerMessagesRead": 1024, 
  "yammerMessagesLiked": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
