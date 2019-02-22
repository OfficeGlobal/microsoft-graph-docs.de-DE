---
title: managedDeviceCleanupSettings-Ressourcentyp
description: Definieren Sie die Regel, wenn der Administrator möchte, dass die Geräte bereinigt werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76abaf4cb06156881a530d50e3322e649eedde51
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148482"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="c7e52-103">managedDeviceCleanupSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c7e52-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="c7e52-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c7e52-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7e52-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c7e52-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7e52-106">Definieren Sie die Regel, wenn der Administrator möchte, dass die Geräte bereinigt werden.</span><span class="sxs-lookup"><span data-stu-id="c7e52-106">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="c7e52-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c7e52-107">Properties</span></span>
|<span data-ttu-id="c7e52-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c7e52-108">Property</span></span>|<span data-ttu-id="c7e52-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c7e52-109">Type</span></span>|<span data-ttu-id="c7e52-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7e52-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7e52-111">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="c7e52-111">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="c7e52-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c7e52-112">String</span></span>|<span data-ttu-id="c7e52-113">Anzahl der Tage, an denen das Gerät InTune nicht kontaktiert hat.</span><span class="sxs-lookup"><span data-stu-id="c7e52-113">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7e52-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c7e52-114">Relationships</span></span>
<span data-ttu-id="c7e52-115">Keine</span><span class="sxs-lookup"><span data-stu-id="c7e52-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7e52-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c7e52-116">JSON Representation</span></span>
<span data-ttu-id="c7e52-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c7e52-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceCleanupSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCleanupSettings",
  "deviceInactivityBeforeRetirementInDays": "String"
}
```




