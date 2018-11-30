---
title: Ressourcentyp office365GroupsActivityStorage
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 23ff4d112373f52c4c19d6631ac89bac22399b29
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064924"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="1379b-103">Ressourcentyp office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="1379b-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1379b-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1379b-104">Properties</span></span>

| <span data-ttu-id="1379b-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1379b-105">Property</span></span>                  | <span data-ttu-id="1379b-106">Typ</span><span class="sxs-lookup"><span data-stu-id="1379b-106">Type</span></span>   | <span data-ttu-id="1379b-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1379b-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="1379b-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1379b-108">reportRefreshDate</span></span>         | <span data-ttu-id="1379b-109">Datum</span><span class="sxs-lookup"><span data-stu-id="1379b-109">Date</span></span>   | <span data-ttu-id="1379b-110">Das aktuelle Datum des Inhalts.</span><span class="sxs-lookup"><span data-stu-id="1379b-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="1379b-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="1379b-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="1379b-112">Int64</span><span class="sxs-lookup"><span data-stu-id="1379b-112">Int64</span></span>  | <span data-ttu-id="1379b-113">Der Speicher, die in der Gruppenpostfach verwendet.</span><span class="sxs-lookup"><span data-stu-id="1379b-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="1379b-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="1379b-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="1379b-115">Int64</span><span class="sxs-lookup"><span data-stu-id="1379b-115">Int64</span></span>  | <span data-ttu-id="1379b-116">Der Speicher in SharePoint-Dokumentbibliothek verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="1379b-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="1379b-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="1379b-117">reportDate</span></span>                | <span data-ttu-id="1379b-118">Datum</span><span class="sxs-lookup"><span data-stu-id="1379b-118">Date</span></span>   | <span data-ttu-id="1379b-119">Das Datum Snapshot für Exchange und SharePoint verwendet Speicher.</span><span class="sxs-lookup"><span data-stu-id="1379b-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="1379b-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1379b-120">reportPeriod</span></span>              | <span data-ttu-id="1379b-121">String</span><span class="sxs-lookup"><span data-stu-id="1379b-121">String</span></span> | <span data-ttu-id="1379b-122">Die Anzahl der Tage, die der Bericht wird behandelt.</span><span class="sxs-lookup"><span data-stu-id="1379b-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="1379b-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1379b-123">JSON representation</span></span>

<span data-ttu-id="1379b-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1379b-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailboxStorageUsedInBytes": 1024, 
  "siteStorageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
