---
title: Ressourcentyp windows10AppsForceUpdateSchedule
description: Zeitplan für die Aktualisierung von Windows 10 Force für Apps
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e0bd9b0963f8547b03243aa7ef791a351dc2b08
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418834"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="365a6-103">Ressourcentyp windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="365a6-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="365a6-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="365a6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="365a6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="365a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="365a6-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="365a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="365a6-107">Zeitplan für die Aktualisierung von Windows 10 Force für Apps</span><span class="sxs-lookup"><span data-stu-id="365a6-107">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="365a6-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="365a6-108">Properties</span></span>
|<span data-ttu-id="365a6-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="365a6-109">Property</span></span>|<span data-ttu-id="365a6-110">Typ</span><span class="sxs-lookup"><span data-stu-id="365a6-110">Type</span></span>|<span data-ttu-id="365a6-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="365a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="365a6-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="365a6-112">startDateTime</span></span>|<span data-ttu-id="365a6-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="365a6-113">DateTimeOffset</span></span>|<span data-ttu-id="365a6-114">Starten Sie die Startzeit für die Force neu.</span><span class="sxs-lookup"><span data-stu-id="365a6-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="365a6-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="365a6-115">recurrence</span></span>|[<span data-ttu-id="365a6-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="365a6-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="365a6-117">Serie planen.</span><span class="sxs-lookup"><span data-stu-id="365a6-117">Recurrence schedule.</span></span> <span data-ttu-id="365a6-118">Mögliche Werte: sind `none`, `daily`, `weekly` und `monthly`.</span><span class="sxs-lookup"><span data-stu-id="365a6-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="365a6-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="365a6-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="365a6-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="365a6-120">Boolean</span></span>|<span data-ttu-id="365a6-121">Bei true wird die Aufgabe sofort ausgeführt, wenn StartDateTime in der Vergangenheit andere Person ist, wird zur nächsten Serie ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="365a6-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="365a6-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="365a6-122">Relationships</span></span>
<span data-ttu-id="365a6-123">Keine</span><span class="sxs-lookup"><span data-stu-id="365a6-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="365a6-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="365a6-124">JSON Representation</span></span>
<span data-ttu-id="365a6-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="365a6-125">Here is a JSON representation of the resource.</span></span>
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




