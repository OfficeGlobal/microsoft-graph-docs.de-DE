---
title: AutomaticUpdateMode Enum-Typ
description: Mögliche Werte für den Modus für automatische Updates.
ms.openlocfilehash: c98927e1c1f66e3bf10fa07496aa54ac91bad20b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016465"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="217cf-103">AutomaticUpdateMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="217cf-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="217cf-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="217cf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="217cf-105">Mögliche Werte für den Modus für automatische Updates.</span><span class="sxs-lookup"><span data-stu-id="217cf-105">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="217cf-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="217cf-106">Members</span></span>
|<span data-ttu-id="217cf-107">Element</span><span class="sxs-lookup"><span data-stu-id="217cf-107">Member</span></span>|<span data-ttu-id="217cf-108">Wert</span><span class="sxs-lookup"><span data-stu-id="217cf-108">Value</span></span>|<span data-ttu-id="217cf-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="217cf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="217cf-110">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="217cf-110">userDefined</span></span>|<span data-ttu-id="217cf-111">0</span><span class="sxs-lookup"><span data-stu-id="217cf-111">0</span></span>|<span data-ttu-id="217cf-112">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="217cf-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="217cf-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="217cf-113">notifyDownload</span></span>|<span data-ttu-id="217cf-114">1</span><span class="sxs-lookup"><span data-stu-id="217cf-114">1</span></span>|<span data-ttu-id="217cf-115">Benachrichtigen Sie auf Download.</span><span class="sxs-lookup"><span data-stu-id="217cf-115">Notify on download.</span></span>|
|<span data-ttu-id="217cf-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="217cf-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="217cf-117">2</span><span class="sxs-lookup"><span data-stu-id="217cf-117">2</span></span>|<span data-ttu-id="217cf-118">Automatische Installation zur Wartungszeit.</span><span class="sxs-lookup"><span data-stu-id="217cf-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="217cf-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="217cf-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="217cf-120">3</span><span class="sxs-lookup"><span data-stu-id="217cf-120">3</span></span>|<span data-ttu-id="217cf-121">Automatische Installation und Wartung jederzeit neu starten.</span><span class="sxs-lookup"><span data-stu-id="217cf-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="217cf-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="217cf-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="217cf-123">4</span><span class="sxs-lookup"><span data-stu-id="217cf-123">4</span></span>|<span data-ttu-id="217cf-124">Automatische Installation und zum geplanten Zeitpunkt neu starten.</span><span class="sxs-lookup"><span data-stu-id="217cf-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="217cf-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="217cf-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="217cf-126">5</span><span class="sxs-lookup"><span data-stu-id="217cf-126">5</span></span>|<span data-ttu-id="217cf-127">Automatische Installation und neu starten Sie, ohne Kontrolle durch den Endbenutzer</span><span class="sxs-lookup"><span data-stu-id="217cf-127">Auto-install and restart without end-user control</span></span>|



