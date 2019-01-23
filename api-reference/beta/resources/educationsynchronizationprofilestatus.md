---
title: Ressourcentyp educationSynchronizationProfileStatus
description: 'Stellt den Synchronisierungsstatus eines Profils Schule Daten-Synchronisierung. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1fd77f48544e5e6bc0c582e4ce9fb2a5b1b6601a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396154"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="97dfb-103">Ressourcentyp educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="97dfb-103">educationSynchronizationProfileStatus resource type</span></span>

> <span data-ttu-id="97dfb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="97dfb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97dfb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="97dfb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97dfb-106">Stellt den Synchronisierungsstatus eines Schule Daten [Synchronisierung Profil](educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="97dfb-106">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="97dfb-107">**Hinweis:** Updates für die **EducationSynchronizationProfileStatus** möglicherweise aufgrund der asynchrone Verarbeitung im Hintergrund Sync verzögert.</span><span class="sxs-lookup"><span data-stu-id="97dfb-107">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="97dfb-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="97dfb-108">Methods</span></span>

| <span data-ttu-id="97dfb-109">Methode</span><span class="sxs-lookup"><span data-stu-id="97dfb-109">Method</span></span> | <span data-ttu-id="97dfb-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="97dfb-110">Return Type</span></span> | <span data-ttu-id="97dfb-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97dfb-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="97dfb-112">Abrufen des Status der Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="97dfb-112">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="97dfb-113">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="97dfb-113">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="97dfb-114">Der Status eines bestimmten Synchronisierungsprofils zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97dfb-114">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="97dfb-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="97dfb-115">Properties</span></span>

| <span data-ttu-id="97dfb-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="97dfb-116">Property</span></span> | <span data-ttu-id="97dfb-117">Typ</span><span class="sxs-lookup"><span data-stu-id="97dfb-117">Type</span></span> | <span data-ttu-id="97dfb-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97dfb-118">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="97dfb-119">**status**</span><span class="sxs-lookup"><span data-stu-id="97dfb-119">**status**</span></span> | <span data-ttu-id="97dfb-120">educationSynchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="97dfb-120">educationSynchronizationStatus</span></span> | <span data-ttu-id="97dfb-121">Der Status der Synchronisierung. Mögliche Werte sind: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span><span class="sxs-lookup"><span data-stu-id="97dfb-121">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="97dfb-122">**lastSynchronizationDateTime**</span><span class="sxs-lookup"><span data-stu-id="97dfb-122">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="97dfb-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97dfb-123">DateTimeOffset</span></span> | <span data-ttu-id="97dfb-124">Gibt die Zeit, die beim letzten Änderung im Verzeichnis beobachtet wurden.</span><span class="sxs-lookup"><span data-stu-id="97dfb-124">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="97dfb-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="97dfb-125">JSON representation</span></span>
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
