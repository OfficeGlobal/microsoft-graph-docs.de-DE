---
title: Ressourcentyp windows10AppsForceUpdateSchedule
description: Zeitplan für die Aktualisierung von Windows 10 Force für Apps
ms.openlocfilehash: 89bbee05c3a76df6999c0d3d16caa591f903c45a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062050"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="9c695-103">Ressourcentyp windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="9c695-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="9c695-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9c695-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c695-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9c695-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c695-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9c695-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c695-107">Zeitplan für die Aktualisierung von Windows 10 Force für Apps</span><span class="sxs-lookup"><span data-stu-id="9c695-107">Windows 10 force update schedule for Apps</span></span>
## <a name="properties"></a><span data-ttu-id="9c695-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9c695-108">Properties</span></span>
|<span data-ttu-id="9c695-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9c695-109">Property</span></span>|<span data-ttu-id="9c695-110">Typ</span><span class="sxs-lookup"><span data-stu-id="9c695-110">Type</span></span>|<span data-ttu-id="9c695-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c695-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c695-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9c695-112">startDateTime</span></span>|<span data-ttu-id="9c695-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c695-113">DateTimeOffset</span></span>|<span data-ttu-id="9c695-114">Starten Sie die Startzeit für die Force neu.</span><span class="sxs-lookup"><span data-stu-id="9c695-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="9c695-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="9c695-115">recurrence</span></span>|[<span data-ttu-id="9c695-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="9c695-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="9c695-117">Serie planen.</span><span class="sxs-lookup"><span data-stu-id="9c695-117">Recurrence schedule.</span></span> <span data-ttu-id="9c695-118">Mögliche Werte: sind `none`, `daily`, `weekly` und `monthly`.</span><span class="sxs-lookup"><span data-stu-id="9c695-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="9c695-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="9c695-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="9c695-120">Boolesch</span><span class="sxs-lookup"><span data-stu-id="9c695-120">Boolean</span></span>|<span data-ttu-id="9c695-121">Bei true wird die Aufgabe sofort ausgeführt, wenn StartDateTime in der Vergangenheit andere Person ist, wird zur nächsten Serie ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="9c695-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c695-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9c695-122">Relationships</span></span>
<span data-ttu-id="9c695-123">Keine</span><span class="sxs-lookup"><span data-stu-id="9c695-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9c695-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9c695-124">JSON Representation</span></span>
<span data-ttu-id="9c695-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9c695-125">Here is a JSON representation of the resource.</span></span>
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





