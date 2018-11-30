---
title: deviceManagementSettings-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: 81aa176af23451675b58a916e9b092ef119dfcb3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060576"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="d243b-103">deviceManagementSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d243b-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="d243b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d243b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d243b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d243b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d243b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d243b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d243b-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="d243b-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="d243b-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d243b-108">Properties</span></span>
|<span data-ttu-id="d243b-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d243b-109">Property</span></span>|<span data-ttu-id="d243b-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d243b-110">Type</span></span>|<span data-ttu-id="d243b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d243b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d243b-112">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="d243b-112">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="d243b-113">Int32</span><span class="sxs-lookup"><span data-stu-id="d243b-113">Int32</span></span>|<span data-ttu-id="d243b-114">Die Anzahl von Tagen, die ein Gerät ohne Einchecken konform bleiben kann.</span><span class="sxs-lookup"><span data-stu-id="d243b-114">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="d243b-115">Gültige Werte: 0 bis 120</span><span class="sxs-lookup"><span data-stu-id="d243b-115">Valid values 0 to 120</span></span>|
|<span data-ttu-id="d243b-116">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="d243b-116">isScheduledActionEnabled</span></span>|<span data-ttu-id="d243b-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="d243b-117">Boolean</span></span>|<span data-ttu-id="d243b-118">Gibt an, ob das Feature für eine geplante Aktion für die Regel aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="d243b-118">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="d243b-119">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="d243b-119">secureByDefault</span></span>|<span data-ttu-id="d243b-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="d243b-120">Boolean</span></span>|<span data-ttu-id="d243b-121">Ist dies auf „true“ gesetzt, sollte das Gerät als nicht konform gelten, wenn keine Konformitätsrichtlinie verfolgt wird.</span><span class="sxs-lookup"><span data-stu-id="d243b-121">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="d243b-122">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="d243b-122">enhancedJailBreak</span></span>|<span data-ttu-id="d243b-123">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d243b-123">Boolean</span></span>|<span data-ttu-id="d243b-124">Ist Feature aktiviert ist oder nicht erweiterten Jailbreak Erkennung.</span><span class="sxs-lookup"><span data-stu-id="d243b-124">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="d243b-125">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="d243b-125">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="d243b-126">Int32</span><span class="sxs-lookup"><span data-stu-id="d243b-126">Int32</span></span>|<span data-ttu-id="d243b-127">Wenn das Gerät nicht prüft für die angegebene Anzahl von Tagen, möglicherweise die Mandantendaten entfernt, und das Gerät werden nicht in die Verwaltung.</span><span class="sxs-lookup"><span data-stu-id="d243b-127">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="d243b-128">Gültige Werte 30 bis 270</span><span class="sxs-lookup"><span data-stu-id="d243b-128">Valid values 30 to 270</span></span>|

## <a name="relationships"></a><span data-ttu-id="d243b-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d243b-129">Relationships</span></span>
<span data-ttu-id="d243b-130">Keine</span><span class="sxs-lookup"><span data-stu-id="d243b-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d243b-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d243b-131">JSON Representation</span></span>
<span data-ttu-id="d243b-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d243b-132">Here is a JSON representation of the resource.</span></span>
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





