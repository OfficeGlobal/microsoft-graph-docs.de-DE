---
title: sharedPCAccountManagerPolicy-Ressourcentyp
description: SharedPC-Konto-Manager-Richtlinie. Gilt nur, wenn der Konto-Manager aktiviert ist.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 683915fdf1a0878e72229ed98cca457fbf77082d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260095"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="eefe6-104">sharedPCAccountManagerPolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="eefe6-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="eefe6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="eefe6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eefe6-106">SharedPC-Konto-Manager-Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="eefe6-106">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="eefe6-107">Gilt nur, wenn der Konto-Manager aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="eefe6-107">Only applies when the account manager is enabled.</span></span>

## <a name="properties"></a><span data-ttu-id="eefe6-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="eefe6-108">Properties</span></span>
|<span data-ttu-id="eefe6-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eefe6-109">Property</span></span>|<span data-ttu-id="eefe6-110">Typ</span><span class="sxs-lookup"><span data-stu-id="eefe6-110">Type</span></span>|<span data-ttu-id="eefe6-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eefe6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eefe6-112">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="eefe6-112">accountDeletionPolicy</span></span>|[<span data-ttu-id="eefe6-113">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="eefe6-113">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="eefe6-114">Konfiguriert, wann Konten gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="eefe6-114">Configures when accounts are deleted.</span></span> <span data-ttu-id="eefe6-115">Mögliche Werte sind: `immediate`, `diskSpaceThreshold` und `diskSpaceThresholdOrInactiveThreshold`.</span><span class="sxs-lookup"><span data-stu-id="eefe6-115">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="eefe6-116">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="eefe6-116">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="eefe6-117">Int32</span><span class="sxs-lookup"><span data-stu-id="eefe6-117">Int32</span></span>|<span data-ttu-id="eefe6-118">Legt den Prozentsatz des verfügbaren Speicherplatzes fest, den ein PC haben sollte, damit keine weiteren zwischengespeicherten freigegebenen PC-Konten gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="eefe6-118">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="eefe6-119">Gilt nur, wenn AccountDeletionPolicy den Wert DiskSpaceThreshold oder DiskSpaceThresholdOrInactiveThreshold hat.</span><span class="sxs-lookup"><span data-stu-id="eefe6-119">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="eefe6-120">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="eefe6-120">Valid values 0 to 100</span></span>|
|<span data-ttu-id="eefe6-121">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="eefe6-121">inactiveThresholdDays</span></span>|<span data-ttu-id="eefe6-122">Int32</span><span class="sxs-lookup"><span data-stu-id="eefe6-122">Int32</span></span>|<span data-ttu-id="eefe6-123">Gibt an, wann mit dem Löschen von Konten begonnen wird, wenn während des angegebenen Zeitraums (Anzahl von Tagen) keine Anmeldung stattgefunden hat.</span><span class="sxs-lookup"><span data-stu-id="eefe6-123">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="eefe6-124">Gilt nur, wenn AccountDeletionPolicy den Wert DiskSpaceThreshold oder DiskSpaceThresholdOrInactiveThreshold hat.</span><span class="sxs-lookup"><span data-stu-id="eefe6-124">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="eefe6-125">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="eefe6-125">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="eefe6-126">Int32</span><span class="sxs-lookup"><span data-stu-id="eefe6-126">Int32</span></span>|<span data-ttu-id="eefe6-127">Legt den auf einem PC verbleibenden Prozentsatz an Speicherplatz fest, ab dem Konten im Cache gelöscht werden, um Speicherplatz freizugeben.</span><span class="sxs-lookup"><span data-stu-id="eefe6-127">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="eefe6-128">Konten, die am längsten inaktiv waren, werden zuerst gelöscht.</span><span class="sxs-lookup"><span data-stu-id="eefe6-128">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="eefe6-129">Gilt nur, wenn AccountDeletionPolicy den Wert DiskSpaceThresholdOrInactiveThreshold hat.</span><span class="sxs-lookup"><span data-stu-id="eefe6-129">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="eefe6-130">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="eefe6-130">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="eefe6-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="eefe6-131">Relationships</span></span>
<span data-ttu-id="eefe6-132">Keine</span><span class="sxs-lookup"><span data-stu-id="eefe6-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eefe6-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="eefe6-133">JSON Representation</span></span>
<span data-ttu-id="eefe6-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="eefe6-134">Here is a JSON representation of the resource.</span></span>
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



