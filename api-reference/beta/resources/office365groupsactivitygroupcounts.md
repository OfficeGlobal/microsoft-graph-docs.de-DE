---
title: Ressourcentyp office365GroupsActivityGroupCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 12dc0121c8f37c694265fce0d6cb5f58e56e0966
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060833"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="cceb5-103">Ressourcentyp office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="cceb5-103">office365GroupsActivityGroupCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="cceb5-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cceb5-104">Properties</span></span>

| <span data-ttu-id="cceb5-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cceb5-105">Property</span></span>          | <span data-ttu-id="cceb5-106">Typ</span><span class="sxs-lookup"><span data-stu-id="cceb5-106">Type</span></span>   | <span data-ttu-id="cceb5-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cceb5-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="cceb5-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="cceb5-108">reportRefreshDate</span></span> | <span data-ttu-id="cceb5-109">Datum</span><span class="sxs-lookup"><span data-stu-id="cceb5-109">Date</span></span>   | <span data-ttu-id="cceb5-110">Das aktuelle Datum des Inhalts.</span><span class="sxs-lookup"><span data-stu-id="cceb5-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="cceb5-111">gesamt</span><span class="sxs-lookup"><span data-stu-id="cceb5-111">total</span></span>             | <span data-ttu-id="cceb5-112">Int64</span><span class="sxs-lookup"><span data-stu-id="cceb5-112">Int64</span></span>  | <span data-ttu-id="cceb5-113">Die Gesamtzahl der Gruppen.</span><span class="sxs-lookup"><span data-stu-id="cceb5-113">The total number of groups.</span></span>              |
| <span data-ttu-id="cceb5-114">aktive</span><span class="sxs-lookup"><span data-stu-id="cceb5-114">active</span></span>            | <span data-ttu-id="cceb5-115">Int64</span><span class="sxs-lookup"><span data-stu-id="cceb5-115">Int64</span></span>  | <span data-ttu-id="cceb5-116">Die Anzahl der aktiven Gruppen.</span><span class="sxs-lookup"><span data-stu-id="cceb5-116">The number of active groups.</span></span> <span data-ttu-id="cceb5-117">Eine Gruppe wird als aktiv betrachtet, wenn eines der folgenden aufgetreten ist: Postfach empfangene e-Mails; gruppieren Benutzer angezeigt, bearbeitet, freigegebene oder Dateien in SharePoint-Dokumentbibliothek synchronisiert; SharePoint-Seiten angezeigt; Benutzer gebucht, lesen oder gefallen Nachrichten in Yammer-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="cceb5-117">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="cceb5-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="cceb5-118">reportDate</span></span>        | <span data-ttu-id="cceb5-119">Datum</span><span class="sxs-lookup"><span data-stu-id="cceb5-119">Date</span></span>   | <span data-ttu-id="cceb5-120">Das Datum, an dem eine Anzahl von Gruppen aktiv waren.</span><span class="sxs-lookup"><span data-stu-id="cceb5-120">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="cceb5-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="cceb5-121">reportPeriod</span></span>      | <span data-ttu-id="cceb5-122">String</span><span class="sxs-lookup"><span data-stu-id="cceb5-122">String</span></span> | <span data-ttu-id="cceb5-123">Die Anzahl der Tage, die der Bericht wird behandelt.</span><span class="sxs-lookup"><span data-stu-id="cceb5-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="cceb5-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cceb5-124">JSON representation</span></span>

<span data-ttu-id="cceb5-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cceb5-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityGroupCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
