---
title: windows10AppsForceUpdateSchedule-Ressourcentyp
description: Windows 10 Erzwingen des Aktualisierungszeitplans für apps
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7aa5573c3d644299b9c0aa424f348a67db8379d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158226"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="78059-103">windows10AppsForceUpdateSchedule-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="78059-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="78059-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="78059-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78059-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="78059-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78059-106">Windows 10 Erzwingen des Aktualisierungszeitplans für apps</span><span class="sxs-lookup"><span data-stu-id="78059-106">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="78059-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="78059-107">Properties</span></span>
|<span data-ttu-id="78059-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="78059-108">Property</span></span>|<span data-ttu-id="78059-109">Typ</span><span class="sxs-lookup"><span data-stu-id="78059-109">Type</span></span>|<span data-ttu-id="78059-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78059-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78059-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="78059-111">startDateTime</span></span>|<span data-ttu-id="78059-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78059-112">DateTimeOffset</span></span>|<span data-ttu-id="78059-113">Die Startzeit des erzwungenen Neustarts.</span><span class="sxs-lookup"><span data-stu-id="78059-113">The start time for the force restart.</span></span>|
|<span data-ttu-id="78059-114">recurrence</span><span class="sxs-lookup"><span data-stu-id="78059-114">recurrence</span></span>|[<span data-ttu-id="78059-115">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="78059-115">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="78059-116">Serienzeitplan.</span><span class="sxs-lookup"><span data-stu-id="78059-116">Recurrence schedule.</span></span> <span data-ttu-id="78059-117">Mögliche Werte: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="78059-117">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="78059-118">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="78059-118">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="78059-119">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="78059-119">Boolean</span></span>|<span data-ttu-id="78059-120">Wenn true, wird die Aufgabe sofort ausgeführt, wenn StartDateTime in der Vergangenheit ist, andernfalls wird bei der nächsten Serie ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="78059-120">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78059-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="78059-121">Relationships</span></span>
<span data-ttu-id="78059-122">Keine</span><span class="sxs-lookup"><span data-stu-id="78059-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78059-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="78059-123">JSON Representation</span></span>
<span data-ttu-id="78059-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="78059-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AppsForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "runImmediatelyIfAfterStartDateTime": true
}
```




