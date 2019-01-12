---
title: deviceManagementSettings-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fda8ac13e97f7c5dd6ed1efda0443b2f898c91c8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959013"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="7582b-103">deviceManagementSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7582b-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="7582b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7582b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7582b-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="7582b-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="7582b-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7582b-106">Properties</span></span>
|<span data-ttu-id="7582b-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7582b-107">Property</span></span>|<span data-ttu-id="7582b-108">Typ</span><span class="sxs-lookup"><span data-stu-id="7582b-108">Type</span></span>|<span data-ttu-id="7582b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7582b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7582b-110">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="7582b-110">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="7582b-111">Int32</span><span class="sxs-lookup"><span data-stu-id="7582b-111">Int32</span></span>|<span data-ttu-id="7582b-112">Die Anzahl von Tagen, die ein Gerät ohne Einchecken konform bleiben kann.</span><span class="sxs-lookup"><span data-stu-id="7582b-112">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="7582b-113">Gültige Werte: 0 bis 120</span><span class="sxs-lookup"><span data-stu-id="7582b-113">Valid values 0 to 120</span></span>|
|<span data-ttu-id="7582b-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="7582b-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="7582b-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="7582b-115">Boolean</span></span>|<span data-ttu-id="7582b-116">Gibt an, ob das Feature für eine geplante Aktion für die Regel aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="7582b-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="7582b-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="7582b-117">secureByDefault</span></span>|<span data-ttu-id="7582b-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="7582b-118">Boolean</span></span>|<span data-ttu-id="7582b-119">Ist dies auf „true“ gesetzt, sollte das Gerät als nicht konform gelten, wenn keine Konformitätsrichtlinie verfolgt wird.</span><span class="sxs-lookup"><span data-stu-id="7582b-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="7582b-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7582b-120">Relationships</span></span>
<span data-ttu-id="7582b-121">Keine</span><span class="sxs-lookup"><span data-stu-id="7582b-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7582b-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7582b-122">JSON Representation</span></span>
<span data-ttu-id="7582b-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7582b-123">Here is a JSON representation of the resource.</span></span>
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



