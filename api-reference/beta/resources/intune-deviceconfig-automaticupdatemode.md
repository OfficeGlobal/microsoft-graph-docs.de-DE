---
title: Eigenschaften automaticupdatemode-Enumerationstyp
description: Mögliche Werte für den automatischen Aktualisierungsmodus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bba7addc5ae3b7942c3e52e1d8989100e27b2831
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156784"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="f3dc7-103">Eigenschaften automaticupdatemode-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="f3dc7-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="f3dc7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3dc7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3dc7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f3dc7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3dc7-106">Mögliche Werte für den automatischen Aktualisierungsmodus.</span><span class="sxs-lookup"><span data-stu-id="f3dc7-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="f3dc7-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="f3dc7-107">Members</span></span>
|<span data-ttu-id="f3dc7-108">Element</span><span class="sxs-lookup"><span data-stu-id="f3dc7-108">Member</span></span>|<span data-ttu-id="f3dc7-109">Wert</span><span class="sxs-lookup"><span data-stu-id="f3dc7-109">Value</span></span>|<span data-ttu-id="f3dc7-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3dc7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3dc7-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="f3dc7-111">userDefined</span></span>|<span data-ttu-id="f3dc7-112">0</span><span class="sxs-lookup"><span data-stu-id="f3dc7-112">0</span></span>|<span data-ttu-id="f3dc7-113">Benutzerdefiniert, Standardwert, keine Absicht.</span><span class="sxs-lookup"><span data-stu-id="f3dc7-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="f3dc7-114">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="f3dc7-114">notifyDownload</span></span>|<span data-ttu-id="f3dc7-115">1</span><span class="sxs-lookup"><span data-stu-id="f3dc7-115">1</span></span>|<span data-ttu-id="f3dc7-116">Benachrichtigung beim Download.</span><span class="sxs-lookup"><span data-stu-id="f3dc7-116">Notify on download.</span></span>|
|<span data-ttu-id="f3dc7-117">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="f3dc7-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="f3dc7-118">2</span><span class="sxs-lookup"><span data-stu-id="f3dc7-118">2</span></span>|<span data-ttu-id="f3dc7-119">Automatische Installation zur Wartungszeit.</span><span class="sxs-lookup"><span data-stu-id="f3dc7-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="f3dc7-120">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="f3dc7-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="f3dc7-121">3</span><span class="sxs-lookup"><span data-stu-id="f3dc7-121">3</span></span>|<span data-ttu-id="f3dc7-122">Automatisches Installieren und Neustarten zum Zeitpunkt der Wartung.</span><span class="sxs-lookup"><span data-stu-id="f3dc7-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="f3dc7-123">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="f3dc7-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="f3dc7-124">4</span><span class="sxs-lookup"><span data-stu-id="f3dc7-124">4</span></span>|<span data-ttu-id="f3dc7-125">Automatisches Installieren und Neustarten zum geplanten Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="f3dc7-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="f3dc7-126">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="f3dc7-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="f3dc7-127">5</span><span class="sxs-lookup"><span data-stu-id="f3dc7-127">5</span></span>|<span data-ttu-id="f3dc7-128">Automatisches Installieren und Neustarten ohne Endbenutzer Steuerelement</span><span class="sxs-lookup"><span data-stu-id="f3dc7-128">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="f3dc7-129">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="f3dc7-129">windowsDefault</span></span>|<span data-ttu-id="f3dc7-130">6</span><span class="sxs-lookup"><span data-stu-id="f3dc7-130">6</span></span>|<span data-ttu-id="f3dc7-131">Zurücksetzen auf Windows-Standardwert.</span><span class="sxs-lookup"><span data-stu-id="f3dc7-131">Reset to Windows default value.</span></span>|




