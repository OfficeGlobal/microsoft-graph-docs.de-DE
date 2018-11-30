---
title: Ressourcentyp educationSynchronizationProfileStatus
description: 'Stellt den Synchronisierungsstatus eines Profils Schule Daten-Synchronisierung. '
ms.openlocfilehash: 6d2c638e1f92a6c3e090cb2bf3bb55e8482bbc4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065947"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="710f3-103">Ressourcentyp educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="710f3-103">educationSynchronizationProfileStatus resource type</span></span>

> <span data-ttu-id="710f3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="710f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="710f3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="710f3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="710f3-106">Stellt den Synchronisierungsstatus eines Schule Daten [Synchronisierung Profil](educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="710f3-106">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="710f3-107">**Hinweis:** Updates für die **EducationSynchronizationProfileStatus** möglicherweise aufgrund der asynchrone Verarbeitung im Hintergrund Sync verzögert.</span><span class="sxs-lookup"><span data-stu-id="710f3-107">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="710f3-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="710f3-108">Methods</span></span>

| <span data-ttu-id="710f3-109">Methode</span><span class="sxs-lookup"><span data-stu-id="710f3-109">Method</span></span> | <span data-ttu-id="710f3-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="710f3-110">Return Type</span></span> | <span data-ttu-id="710f3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="710f3-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="710f3-112">Abrufen des Status der Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="710f3-112">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="710f3-113">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="710f3-113">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="710f3-114">Der Status eines bestimmten Synchronisierungsprofils zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="710f3-114">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="710f3-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="710f3-115">Properties</span></span>

| <span data-ttu-id="710f3-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="710f3-116">Property</span></span> | <span data-ttu-id="710f3-117">Typ</span><span class="sxs-lookup"><span data-stu-id="710f3-117">Type</span></span> | <span data-ttu-id="710f3-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="710f3-118">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="710f3-119">**status**</span><span class="sxs-lookup"><span data-stu-id="710f3-119">**status**</span></span> | <span data-ttu-id="710f3-120">string</span><span class="sxs-lookup"><span data-stu-id="710f3-120">string</span></span> | <span data-ttu-id="710f3-121">Der Status der Synchronisierung. Mögliche Werte sind: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span><span class="sxs-lookup"><span data-stu-id="710f3-121">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="710f3-122">**lastSynchronizationDateTime**</span><span class="sxs-lookup"><span data-stu-id="710f3-122">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="710f3-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="710f3-123">DateTimeOffset</span></span> | <span data-ttu-id="710f3-124">Gibt die Zeit, die beim letzten Änderung im Verzeichnis beobachtet wurden.</span><span class="sxs-lookup"><span data-stu-id="710f3-124">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="710f3-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="710f3-125">JSON representation</span></span>
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