---
title: Ressourcentyp educationSynchronizationProfileStatus
description: 'Stellt den Synchronisierungsstatus eines Profils Schule Daten-Synchronisierung. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 12908f6454cb27c673935f1e4c64c921b7ff0dcd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523540"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="cb2ea-103">Ressourcentyp educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="cb2ea-103">educationSynchronizationProfileStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb2ea-104">Stellt den Synchronisierungsstatus eines Schule Daten [Synchronisierung Profil](educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="cb2ea-104">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="cb2ea-105">**Hinweis:** Updates für die **EducationSynchronizationProfileStatus** möglicherweise aufgrund der asynchrone Verarbeitung im Hintergrund Sync verzögert.</span><span class="sxs-lookup"><span data-stu-id="cb2ea-105">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="cb2ea-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="cb2ea-106">Methods</span></span>

| <span data-ttu-id="cb2ea-107">Methode</span><span class="sxs-lookup"><span data-stu-id="cb2ea-107">Method</span></span> | <span data-ttu-id="cb2ea-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="cb2ea-108">Return Type</span></span> | <span data-ttu-id="cb2ea-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb2ea-109">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="cb2ea-110">Abrufen des Status der Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="cb2ea-110">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="cb2ea-111">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="cb2ea-111">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="cb2ea-112">Der Status eines bestimmten Synchronisierungsprofils zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb2ea-112">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="cb2ea-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cb2ea-113">Properties</span></span>

| <span data-ttu-id="cb2ea-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cb2ea-114">Property</span></span> | <span data-ttu-id="cb2ea-115">Typ</span><span class="sxs-lookup"><span data-stu-id="cb2ea-115">Type</span></span> | <span data-ttu-id="cb2ea-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb2ea-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="cb2ea-117">**status**</span><span class="sxs-lookup"><span data-stu-id="cb2ea-117">**status**</span></span> | <span data-ttu-id="cb2ea-118">educationSynchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="cb2ea-118">educationSynchronizationStatus</span></span> | <span data-ttu-id="cb2ea-119">Der Status der Synchronisierung. Mögliche Werte sind: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span><span class="sxs-lookup"><span data-stu-id="cb2ea-119">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="cb2ea-120">**lastSynchronizationDateTime**</span><span class="sxs-lookup"><span data-stu-id="cb2ea-120">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="cb2ea-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb2ea-121">DateTimeOffset</span></span> | <span data-ttu-id="cb2ea-122">Gibt die Zeit, die beim letzten Änderung im Verzeichnis beobachtet wurden.</span><span class="sxs-lookup"><span data-stu-id="cb2ea-122">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="cb2ea-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cb2ea-123">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationprofilestatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
