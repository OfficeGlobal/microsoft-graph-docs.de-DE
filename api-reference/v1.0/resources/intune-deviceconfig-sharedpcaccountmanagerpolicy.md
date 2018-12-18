---
title: sharedPCAccountManagerPolicy-Ressourcentyp
description: SharedPC-Konto-Manager-Richtlinie. Gilt nur, wenn der Konto-Manager aktiviert ist.
author: tfitzmac
ms.openlocfilehash: 7eafffbfac115c95cbf2c62be630cf7958965ce9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306566"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="8f9d9-104">sharedPCAccountManagerPolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8f9d9-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="8f9d9-105">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8f9d9-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f9d9-106">SharedPC-Konto-Manager-Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="8f9d9-106">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="8f9d9-107">Gilt nur, wenn der Konto-Manager aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="8f9d9-107">Only applies when the account manager is enabled.</span></span>
## <a name="properties"></a><span data-ttu-id="8f9d9-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8f9d9-108">Properties</span></span>
|<span data-ttu-id="8f9d9-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8f9d9-109">Property</span></span>|<span data-ttu-id="8f9d9-110">Typ</span><span class="sxs-lookup"><span data-stu-id="8f9d9-110">Type</span></span>|<span data-ttu-id="8f9d9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f9d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f9d9-112">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="8f9d9-112">accountDeletionPolicy</span></span>|[<span data-ttu-id="8f9d9-113">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="8f9d9-113">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="8f9d9-114">Konfiguriert, wann Konten gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="8f9d9-114">Configures when accounts are deleted.</span></span> <span data-ttu-id="8f9d9-115">Mögliche Werte sind: `immediate`, `diskSpaceThreshold` und `diskSpaceThresholdOrInactiveThreshold`.</span><span class="sxs-lookup"><span data-stu-id="8f9d9-115">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="8f9d9-116">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="8f9d9-116">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="8f9d9-117">Int32</span><span class="sxs-lookup"><span data-stu-id="8f9d9-117">Int32</span></span>|<span data-ttu-id="8f9d9-118">Legt den Prozentsatz des verfügbaren Speicherplatzes fest, den ein PC haben sollte, damit keine weiteren zwischengespeicherten freigegebenen PC-Konten gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="8f9d9-118">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="8f9d9-119">Gilt nur, wenn AccountDeletionPolicy den Wert DiskSpaceThreshold oder DiskSpaceThresholdOrInactiveThreshold hat.</span><span class="sxs-lookup"><span data-stu-id="8f9d9-119">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="8f9d9-120">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="8f9d9-120">Valid values 0 to 100</span></span>|
|<span data-ttu-id="8f9d9-121">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="8f9d9-121">inactiveThresholdDays</span></span>|<span data-ttu-id="8f9d9-122">Int32</span><span class="sxs-lookup"><span data-stu-id="8f9d9-122">Int32</span></span>|<span data-ttu-id="8f9d9-123">Gibt an, wann mit dem Löschen von Konten begonnen wird, wenn während des angegebenen Zeitraums (Anzahl von Tagen) keine Anmeldung stattgefunden hat.</span><span class="sxs-lookup"><span data-stu-id="8f9d9-123">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="8f9d9-124">Gilt nur, wenn AccountDeletionPolicy den Wert DiskSpaceThreshold oder DiskSpaceThresholdOrInactiveThreshold hat.</span><span class="sxs-lookup"><span data-stu-id="8f9d9-124">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="8f9d9-125">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="8f9d9-125">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="8f9d9-126">Int32</span><span class="sxs-lookup"><span data-stu-id="8f9d9-126">Int32</span></span>|<span data-ttu-id="8f9d9-127">Legt den auf einem PC verbleibenden Prozentsatz an Speicherplatz fest, ab dem Konten im Cache gelöscht werden, um Speicherplatz freizugeben.</span><span class="sxs-lookup"><span data-stu-id="8f9d9-127">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="8f9d9-128">Konten, die am längsten inaktiv waren, werden zuerst gelöscht.</span><span class="sxs-lookup"><span data-stu-id="8f9d9-128">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="8f9d9-129">Gilt nur, wenn AccountDeletionPolicy den Wert DiskSpaceThresholdOrInactiveThreshold hat.</span><span class="sxs-lookup"><span data-stu-id="8f9d9-129">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="8f9d9-130">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="8f9d9-130">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f9d9-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8f9d9-131">Relationships</span></span>
<span data-ttu-id="8f9d9-132">Keine</span><span class="sxs-lookup"><span data-stu-id="8f9d9-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8f9d9-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8f9d9-133">JSON Representation</span></span>
<span data-ttu-id="8f9d9-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8f9d9-134">Here is a JSON representation of the resource.</span></span>
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



