---
title: Ressourcentyp educationSynchronizationProfileStatus
description: 'Stellt den Synchronisierungsstatus eines Profils Schule Daten-Synchronisierung. '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 4476ffc7c64fb5d9852c46e2b748587e79d427c1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858163"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="6af46-103">Ressourcentyp educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="6af46-103">educationSynchronizationProfileStatus resource type</span></span>

> <span data-ttu-id="6af46-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6af46-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6af46-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6af46-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6af46-106">Stellt den Synchronisierungsstatus eines Schule Daten [Synchronisierung Profil](educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="6af46-106">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="6af46-107">**Hinweis:** Updates für die **EducationSynchronizationProfileStatus** möglicherweise aufgrund der asynchrone Verarbeitung im Hintergrund Sync verzögert.</span><span class="sxs-lookup"><span data-stu-id="6af46-107">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="6af46-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="6af46-108">Methods</span></span>

| <span data-ttu-id="6af46-109">Methode</span><span class="sxs-lookup"><span data-stu-id="6af46-109">Method</span></span> | <span data-ttu-id="6af46-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6af46-110">Return Type</span></span> | <span data-ttu-id="6af46-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6af46-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="6af46-112">Abrufen des Status der Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="6af46-112">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="6af46-113">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="6af46-113">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="6af46-114">Der Status eines bestimmten Synchronisierungsprofils zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6af46-114">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="6af46-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6af46-115">Properties</span></span>

| <span data-ttu-id="6af46-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6af46-116">Property</span></span> | <span data-ttu-id="6af46-117">Typ</span><span class="sxs-lookup"><span data-stu-id="6af46-117">Type</span></span> | <span data-ttu-id="6af46-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6af46-118">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="6af46-119">**status**</span><span class="sxs-lookup"><span data-stu-id="6af46-119">**status**</span></span> | <span data-ttu-id="6af46-120">string</span><span class="sxs-lookup"><span data-stu-id="6af46-120">string</span></span> | <span data-ttu-id="6af46-121">Der Status der Synchronisierung. Mögliche Werte sind: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span><span class="sxs-lookup"><span data-stu-id="6af46-121">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="6af46-122">**lastSynchronizationDateTime**</span><span class="sxs-lookup"><span data-stu-id="6af46-122">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="6af46-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6af46-123">DateTimeOffset</span></span> | <span data-ttu-id="6af46-124">Gibt die Zeit, die beim letzten Änderung im Verzeichnis beobachtet wurden.</span><span class="sxs-lookup"><span data-stu-id="6af46-124">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="6af46-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6af46-125">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```
