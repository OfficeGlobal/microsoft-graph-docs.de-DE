---
title: deviceManagementSettings-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d36ab0a845450d803b3f0ac3fb0b9ea58cc4d3d3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250796"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="77573-103">deviceManagementSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="77573-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="77573-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="77573-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77573-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="77573-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="77573-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="77573-106">Properties</span></span>
|<span data-ttu-id="77573-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77573-107">Property</span></span>|<span data-ttu-id="77573-108">Typ</span><span class="sxs-lookup"><span data-stu-id="77573-108">Type</span></span>|<span data-ttu-id="77573-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77573-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77573-110">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="77573-110">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="77573-111">Int32</span><span class="sxs-lookup"><span data-stu-id="77573-111">Int32</span></span>|<span data-ttu-id="77573-112">Die Anzahl von Tagen, die ein Gerät ohne Einchecken konform bleiben kann.</span><span class="sxs-lookup"><span data-stu-id="77573-112">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="77573-113">Gültige Werte: 0 bis 120</span><span class="sxs-lookup"><span data-stu-id="77573-113">Valid values 0 to 120</span></span>|
|<span data-ttu-id="77573-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="77573-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="77573-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="77573-115">Boolean</span></span>|<span data-ttu-id="77573-116">Gibt an, ob das Feature für eine geplante Aktion für die Regel aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="77573-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="77573-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="77573-117">secureByDefault</span></span>|<span data-ttu-id="77573-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="77573-118">Boolean</span></span>|<span data-ttu-id="77573-119">Ist dies auf „true“ gesetzt, sollte das Gerät als nicht konform gelten, wenn keine Konformitätsrichtlinie verfolgt wird.</span><span class="sxs-lookup"><span data-stu-id="77573-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="77573-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="77573-120">Relationships</span></span>
<span data-ttu-id="77573-121">Keine</span><span class="sxs-lookup"><span data-stu-id="77573-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77573-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="77573-122">JSON Representation</span></span>
<span data-ttu-id="77573-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="77573-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true
}
```



