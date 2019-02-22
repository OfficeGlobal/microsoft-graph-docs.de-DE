---
title: sharedPCAccountManagerPolicy-Ressourcentyp
description: SharedPC-Konto-Manager-Richtlinie. Gilt nur, wenn der Konto-Manager aktiviert ist.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47864cb6340699c5e1e223739129dcac2cc21dc9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155888"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="224f3-104">sharedPCAccountManagerPolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="224f3-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="224f3-105">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="224f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="224f3-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="224f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="224f3-107">SharedPC-Konto-Manager-Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="224f3-107">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="224f3-108">Gilt nur, wenn der Konto-Manager aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="224f3-108">Only applies when the account manager is enabled.</span></span>

## <a name="properties"></a><span data-ttu-id="224f3-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="224f3-109">Properties</span></span>
|<span data-ttu-id="224f3-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="224f3-110">Property</span></span>|<span data-ttu-id="224f3-111">Typ</span><span class="sxs-lookup"><span data-stu-id="224f3-111">Type</span></span>|<span data-ttu-id="224f3-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="224f3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="224f3-113">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="224f3-113">accountDeletionPolicy</span></span>|[<span data-ttu-id="224f3-114">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="224f3-114">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="224f3-115">Konfiguriert, wann Konten gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="224f3-115">Configures when accounts are deleted.</span></span> <span data-ttu-id="224f3-116">Mögliche Werte sind: `immediate`, `diskSpaceThreshold` und `diskSpaceThresholdOrInactiveThreshold`.</span><span class="sxs-lookup"><span data-stu-id="224f3-116">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="224f3-117">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="224f3-117">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="224f3-118">Int32</span><span class="sxs-lookup"><span data-stu-id="224f3-118">Int32</span></span>|<span data-ttu-id="224f3-119">Legt den Prozentsatz des verfügbaren Speicherplatzes fest, den ein PC haben sollte, damit keine weiteren zwischengespeicherten freigegebenen PC-Konten gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="224f3-119">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="224f3-120">Gilt nur, wenn AccountDeletionPolicy den Wert DiskSpaceThreshold oder DiskSpaceThresholdOrInactiveThreshold hat.</span><span class="sxs-lookup"><span data-stu-id="224f3-120">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="224f3-121">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="224f3-121">Valid values 0 to 100</span></span>|
|<span data-ttu-id="224f3-122">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="224f3-122">inactiveThresholdDays</span></span>|<span data-ttu-id="224f3-123">Int32</span><span class="sxs-lookup"><span data-stu-id="224f3-123">Int32</span></span>|<span data-ttu-id="224f3-124">Gibt an, wann mit dem Löschen von Konten begonnen wird, wenn während des angegebenen Zeitraums (Anzahl von Tagen) keine Anmeldung stattgefunden hat.</span><span class="sxs-lookup"><span data-stu-id="224f3-124">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="224f3-125">Gilt nur, wenn AccountDeletionPolicy den Wert DiskSpaceThreshold oder DiskSpaceThresholdOrInactiveThreshold hat.</span><span class="sxs-lookup"><span data-stu-id="224f3-125">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="224f3-126">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="224f3-126">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="224f3-127">Int32</span><span class="sxs-lookup"><span data-stu-id="224f3-127">Int32</span></span>|<span data-ttu-id="224f3-128">Legt den auf einem PC verbleibenden Prozentsatz an Speicherplatz fest, ab dem Konten im Cache gelöscht werden, um Speicherplatz freizugeben.</span><span class="sxs-lookup"><span data-stu-id="224f3-128">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="224f3-129">Konten, die am längsten inaktiv waren, werden zuerst gelöscht.</span><span class="sxs-lookup"><span data-stu-id="224f3-129">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="224f3-130">Gilt nur, wenn AccountDeletionPolicy den Wert DiskSpaceThresholdOrInactiveThreshold hat.</span><span class="sxs-lookup"><span data-stu-id="224f3-130">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="224f3-131">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="224f3-131">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="224f3-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="224f3-132">Relationships</span></span>
<span data-ttu-id="224f3-133">Keine</span><span class="sxs-lookup"><span data-stu-id="224f3-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="224f3-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="224f3-134">JSON Representation</span></span>
<span data-ttu-id="224f3-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="224f3-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCAccountManagerPolicy",
  "accountDeletionPolicy": "String",
  "cacheAccountsAboveDiskFreePercentage": 1024,
  "inactiveThresholdDays": 1024,
  "removeAccountsBelowDiskFreePercentage": 1024
}
```




