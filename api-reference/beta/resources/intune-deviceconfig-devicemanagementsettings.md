---
title: deviceManagementSettings-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f973f2645b37375641bc536b5ace0fa508fb0b0e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854418"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="0b6fe-103">deviceManagementSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0b6fe-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="0b6fe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0b6fe-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b6fe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0b6fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b6fe-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0b6fe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b6fe-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="0b6fe-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="0b6fe-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0b6fe-108">Properties</span></span>
|<span data-ttu-id="0b6fe-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0b6fe-109">Property</span></span>|<span data-ttu-id="0b6fe-110">Typ</span><span class="sxs-lookup"><span data-stu-id="0b6fe-110">Type</span></span>|<span data-ttu-id="0b6fe-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b6fe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b6fe-112">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="0b6fe-112">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="0b6fe-113">Int32</span><span class="sxs-lookup"><span data-stu-id="0b6fe-113">Int32</span></span>|<span data-ttu-id="0b6fe-114">Die Anzahl von Tagen, die ein Gerät ohne Einchecken konform bleiben kann.</span><span class="sxs-lookup"><span data-stu-id="0b6fe-114">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="0b6fe-115">Gültige Werte: 0 bis 120</span><span class="sxs-lookup"><span data-stu-id="0b6fe-115">Valid values 0 to 120</span></span>|
|<span data-ttu-id="0b6fe-116">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="0b6fe-116">isScheduledActionEnabled</span></span>|<span data-ttu-id="0b6fe-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6fe-117">Boolean</span></span>|<span data-ttu-id="0b6fe-118">Gibt an, ob das Feature für eine geplante Aktion für die Regel aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="0b6fe-118">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="0b6fe-119">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="0b6fe-119">secureByDefault</span></span>|<span data-ttu-id="0b6fe-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6fe-120">Boolean</span></span>|<span data-ttu-id="0b6fe-121">Ist dies auf „true“ gesetzt, sollte das Gerät als nicht konform gelten, wenn keine Konformitätsrichtlinie verfolgt wird.</span><span class="sxs-lookup"><span data-stu-id="0b6fe-121">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="0b6fe-122">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="0b6fe-122">enhancedJailBreak</span></span>|<span data-ttu-id="0b6fe-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6fe-123">Boolean</span></span>|<span data-ttu-id="0b6fe-124">Ist Feature aktiviert ist oder nicht erweiterten Jailbreak Erkennung.</span><span class="sxs-lookup"><span data-stu-id="0b6fe-124">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="0b6fe-125">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="0b6fe-125">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="0b6fe-126">Int32</span><span class="sxs-lookup"><span data-stu-id="0b6fe-126">Int32</span></span>|<span data-ttu-id="0b6fe-127">Wenn das Gerät nicht prüft für die angegebene Anzahl von Tagen, möglicherweise die Mandantendaten entfernt, und das Gerät werden nicht in die Verwaltung.</span><span class="sxs-lookup"><span data-stu-id="0b6fe-127">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="0b6fe-128">Gültige Werte 30 bis 270</span><span class="sxs-lookup"><span data-stu-id="0b6fe-128">Valid values 30 to 270</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b6fe-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0b6fe-129">Relationships</span></span>
<span data-ttu-id="0b6fe-130">Keine</span><span class="sxs-lookup"><span data-stu-id="0b6fe-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0b6fe-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0b6fe-131">JSON Representation</span></span>
<span data-ttu-id="0b6fe-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0b6fe-132">Here is a JSON representation of the resource.</span></span>
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
  "secureByDefault": true,
  "enhancedJailBreak": true,
  "deviceInactivityBeforeRetirementInDay": 1024
}
```





