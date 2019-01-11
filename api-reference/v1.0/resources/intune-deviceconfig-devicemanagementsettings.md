---
title: deviceManagementSettings-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3742262f2d17cdac1344379b39b4891b5b9919ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830590"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="d1969-103">deviceManagementSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d1969-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="d1969-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d1969-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1969-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="d1969-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="d1969-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d1969-106">Properties</span></span>
|<span data-ttu-id="d1969-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d1969-107">Property</span></span>|<span data-ttu-id="d1969-108">Typ</span><span class="sxs-lookup"><span data-stu-id="d1969-108">Type</span></span>|<span data-ttu-id="d1969-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1969-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1969-110">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="d1969-110">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="d1969-111">Int32</span><span class="sxs-lookup"><span data-stu-id="d1969-111">Int32</span></span>|<span data-ttu-id="d1969-112">Die Anzahl von Tagen, die ein Gerät ohne Einchecken konform bleiben kann.</span><span class="sxs-lookup"><span data-stu-id="d1969-112">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="d1969-113">Gültige Werte: 0 bis 120</span><span class="sxs-lookup"><span data-stu-id="d1969-113">Valid values 0 to 120</span></span>|
|<span data-ttu-id="d1969-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="d1969-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="d1969-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1969-115">Boolean</span></span>|<span data-ttu-id="d1969-116">Gibt an, ob das Feature für eine geplante Aktion für die Regel aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="d1969-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="d1969-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="d1969-117">secureByDefault</span></span>|<span data-ttu-id="d1969-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1969-118">Boolean</span></span>|<span data-ttu-id="d1969-119">Ist dies auf „true“ gesetzt, sollte das Gerät als nicht konform gelten, wenn keine Konformitätsrichtlinie verfolgt wird.</span><span class="sxs-lookup"><span data-stu-id="d1969-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1969-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d1969-120">Relationships</span></span>
<span data-ttu-id="d1969-121">Keine</span><span class="sxs-lookup"><span data-stu-id="d1969-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d1969-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d1969-122">JSON Representation</span></span>
<span data-ttu-id="d1969-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d1969-123">Here is a JSON representation of the resource.</span></span>
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



