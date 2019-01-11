---
title: windowsUpdateActiveHoursInstall-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 797cfc0f9279f0ab232991a95714d31ce37211a3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818424"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="0fb48-103">windowsUpdateActiveHoursInstall-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0fb48-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="0fb48-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0fb48-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0fb48-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0fb48-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0fb48-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0fb48-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0fb48-107">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="0fb48-107">Not yet documented</span></span>

<span data-ttu-id="0fb48-108">Erbt von [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="0fb48-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0fb48-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0fb48-109">Properties</span></span>
|<span data-ttu-id="0fb48-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0fb48-110">Property</span></span>|<span data-ttu-id="0fb48-111">Typ</span><span class="sxs-lookup"><span data-stu-id="0fb48-111">Type</span></span>|<span data-ttu-id="0fb48-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0fb48-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fb48-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="0fb48-113">activeHoursStart</span></span>|<span data-ttu-id="0fb48-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0fb48-114">TimeOfDay</span></span>|<span data-ttu-id="0fb48-115">Beginn der aktiven Stunden</span><span class="sxs-lookup"><span data-stu-id="0fb48-115">Active Hours Start</span></span>|
|<span data-ttu-id="0fb48-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="0fb48-116">activeHoursEnd</span></span>|<span data-ttu-id="0fb48-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0fb48-117">TimeOfDay</span></span>|<span data-ttu-id="0fb48-118">Ende der aktiven Stunden</span><span class="sxs-lookup"><span data-stu-id="0fb48-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fb48-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0fb48-119">Relationships</span></span>
<span data-ttu-id="0fb48-120">Keine</span><span class="sxs-lookup"><span data-stu-id="0fb48-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0fb48-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0fb48-121">JSON Representation</span></span>
<span data-ttu-id="0fb48-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0fb48-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateActiveHoursInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateActiveHoursInstall",
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)"
}
```





