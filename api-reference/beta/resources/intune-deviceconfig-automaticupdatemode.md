---
title: AutomaticUpdateMode Enum-Typ
description: Mögliche Werte für den Modus für automatische Updates.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d982c4c9ee524712c212eba1b8b44349d0a70377
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402636"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="5008a-103">AutomaticUpdateMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="5008a-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="5008a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="5008a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5008a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5008a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5008a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5008a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5008a-107">Mögliche Werte für den Modus für automatische Updates.</span><span class="sxs-lookup"><span data-stu-id="5008a-107">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="5008a-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="5008a-108">Members</span></span>
|<span data-ttu-id="5008a-109">Member</span><span class="sxs-lookup"><span data-stu-id="5008a-109">Member</span></span>|<span data-ttu-id="5008a-110">Wert</span><span class="sxs-lookup"><span data-stu-id="5008a-110">Value</span></span>|<span data-ttu-id="5008a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5008a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5008a-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="5008a-112">userDefined</span></span>|<span data-ttu-id="5008a-113">0</span><span class="sxs-lookup"><span data-stu-id="5008a-113">0</span></span>|<span data-ttu-id="5008a-114">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="5008a-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="5008a-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="5008a-115">notifyDownload</span></span>|<span data-ttu-id="5008a-116">1</span><span class="sxs-lookup"><span data-stu-id="5008a-116">1</span></span>|<span data-ttu-id="5008a-117">Benachrichtigen Sie auf Download.</span><span class="sxs-lookup"><span data-stu-id="5008a-117">Notify on download.</span></span>|
|<span data-ttu-id="5008a-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="5008a-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="5008a-119">2</span><span class="sxs-lookup"><span data-stu-id="5008a-119">2</span></span>|<span data-ttu-id="5008a-120">Automatische Installation zur Wartungszeit.</span><span class="sxs-lookup"><span data-stu-id="5008a-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="5008a-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="5008a-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="5008a-122">3</span><span class="sxs-lookup"><span data-stu-id="5008a-122">3</span></span>|<span data-ttu-id="5008a-123">Automatische Installation und Wartung jederzeit neu starten.</span><span class="sxs-lookup"><span data-stu-id="5008a-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="5008a-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="5008a-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="5008a-125">4</span><span class="sxs-lookup"><span data-stu-id="5008a-125">4</span></span>|<span data-ttu-id="5008a-126">Automatische Installation und zum geplanten Zeitpunkt neu starten.</span><span class="sxs-lookup"><span data-stu-id="5008a-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="5008a-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="5008a-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="5008a-128">5</span><span class="sxs-lookup"><span data-stu-id="5008a-128">5</span></span>|<span data-ttu-id="5008a-129">Automatische Installation und neu starten Sie, ohne Kontrolle durch den Endbenutzer</span><span class="sxs-lookup"><span data-stu-id="5008a-129">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="5008a-130">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="5008a-130">windowsDefault</span></span>|<span data-ttu-id="5008a-131">6</span><span class="sxs-lookup"><span data-stu-id="5008a-131">6</span></span>|<span data-ttu-id="5008a-132">Auf Windows-Standardwert zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="5008a-132">Reset to Windows default value.</span></span>|




