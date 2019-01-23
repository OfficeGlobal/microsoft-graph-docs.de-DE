---
title: sharedPCAccountManagerPolicy-Ressourcentyp
description: SharedPC-Konto-Manager-Richtlinie. Gilt nur, wenn der Konto-Manager aktiviert ist.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d6b7e0ab86af78380f85da8ec37c643e662838c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410994"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="77da8-104">sharedPCAccountManagerPolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="77da8-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="77da8-105">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="77da8-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="77da8-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77da8-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77da8-107">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="77da8-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77da8-108">SharedPC-Konto-Manager-Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="77da8-108">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="77da8-109">Gilt nur, wenn der Konto-Manager aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="77da8-109">Only applies when the account manager is enabled.</span></span>

## <a name="properties"></a><span data-ttu-id="77da8-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="77da8-110">Properties</span></span>
|<span data-ttu-id="77da8-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77da8-111">Property</span></span>|<span data-ttu-id="77da8-112">Typ</span><span class="sxs-lookup"><span data-stu-id="77da8-112">Type</span></span>|<span data-ttu-id="77da8-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77da8-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77da8-114">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="77da8-114">accountDeletionPolicy</span></span>|[<span data-ttu-id="77da8-115">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="77da8-115">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="77da8-116">Konfiguriert, wann Konten gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="77da8-116">Configures when accounts are deleted.</span></span> <span data-ttu-id="77da8-117">Mögliche Werte sind: `immediate`, `diskSpaceThreshold` und `diskSpaceThresholdOrInactiveThreshold`.</span><span class="sxs-lookup"><span data-stu-id="77da8-117">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="77da8-118">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="77da8-118">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="77da8-119">Int32</span><span class="sxs-lookup"><span data-stu-id="77da8-119">Int32</span></span>|<span data-ttu-id="77da8-120">Legt den Prozentsatz des verfügbaren Speicherplatzes fest, den ein PC haben sollte, damit keine weiteren zwischengespeicherten freigegebenen PC-Konten gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="77da8-120">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="77da8-121">Gilt nur, wenn AccountDeletionPolicy den Wert DiskSpaceThreshold oder DiskSpaceThresholdOrInactiveThreshold hat.</span><span class="sxs-lookup"><span data-stu-id="77da8-121">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="77da8-122">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="77da8-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="77da8-123">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="77da8-123">inactiveThresholdDays</span></span>|<span data-ttu-id="77da8-124">Int32</span><span class="sxs-lookup"><span data-stu-id="77da8-124">Int32</span></span>|<span data-ttu-id="77da8-125">Gibt an, wann mit dem Löschen von Konten begonnen wird, wenn während des angegebenen Zeitraums (Anzahl von Tagen) keine Anmeldung stattgefunden hat.</span><span class="sxs-lookup"><span data-stu-id="77da8-125">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="77da8-126">Gilt nur, wenn AccountDeletionPolicy den Wert DiskSpaceThreshold oder DiskSpaceThresholdOrInactiveThreshold hat.</span><span class="sxs-lookup"><span data-stu-id="77da8-126">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="77da8-127">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="77da8-127">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="77da8-128">Int32</span><span class="sxs-lookup"><span data-stu-id="77da8-128">Int32</span></span>|<span data-ttu-id="77da8-129">Legt den auf einem PC verbleibenden Prozentsatz an Speicherplatz fest, ab dem Konten im Cache gelöscht werden, um Speicherplatz freizugeben.</span><span class="sxs-lookup"><span data-stu-id="77da8-129">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="77da8-130">Konten, die am längsten inaktiv waren, werden zuerst gelöscht.</span><span class="sxs-lookup"><span data-stu-id="77da8-130">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="77da8-131">Gilt nur, wenn AccountDeletionPolicy den Wert DiskSpaceThresholdOrInactiveThreshold hat.</span><span class="sxs-lookup"><span data-stu-id="77da8-131">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="77da8-132">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="77da8-132">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="77da8-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="77da8-133">Relationships</span></span>
<span data-ttu-id="77da8-134">Keine</span><span class="sxs-lookup"><span data-stu-id="77da8-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77da8-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="77da8-135">JSON Representation</span></span>
<span data-ttu-id="77da8-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="77da8-136">Here is a JSON representation of the resource.</span></span>
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




