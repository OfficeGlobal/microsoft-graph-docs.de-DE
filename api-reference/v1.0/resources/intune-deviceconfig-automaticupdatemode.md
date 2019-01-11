---
title: AutomaticUpdateMode Enum-Typ
description: Mögliche Werte für den Modus für automatische Updates.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 07a6b410289ea6455d0f6756efa7d1ec4d735ce4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849987"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="4ff27-103">AutomaticUpdateMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="4ff27-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="4ff27-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4ff27-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ff27-105">Mögliche Werte für den Modus für automatische Updates.</span><span class="sxs-lookup"><span data-stu-id="4ff27-105">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="4ff27-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="4ff27-106">Members</span></span>
|<span data-ttu-id="4ff27-107">Element</span><span class="sxs-lookup"><span data-stu-id="4ff27-107">Member</span></span>|<span data-ttu-id="4ff27-108">Wert</span><span class="sxs-lookup"><span data-stu-id="4ff27-108">Value</span></span>|<span data-ttu-id="4ff27-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ff27-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ff27-110">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="4ff27-110">userDefined</span></span>|<span data-ttu-id="4ff27-111">0</span><span class="sxs-lookup"><span data-stu-id="4ff27-111">0</span></span>|<span data-ttu-id="4ff27-112">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="4ff27-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="4ff27-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="4ff27-113">notifyDownload</span></span>|<span data-ttu-id="4ff27-114">1</span><span class="sxs-lookup"><span data-stu-id="4ff27-114">1</span></span>|<span data-ttu-id="4ff27-115">Benachrichtigen Sie auf Download.</span><span class="sxs-lookup"><span data-stu-id="4ff27-115">Notify on download.</span></span>|
|<span data-ttu-id="4ff27-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="4ff27-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="4ff27-117">2</span><span class="sxs-lookup"><span data-stu-id="4ff27-117">2</span></span>|<span data-ttu-id="4ff27-118">Automatische Installation zur Wartungszeit.</span><span class="sxs-lookup"><span data-stu-id="4ff27-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="4ff27-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="4ff27-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="4ff27-120">3</span><span class="sxs-lookup"><span data-stu-id="4ff27-120">3</span></span>|<span data-ttu-id="4ff27-121">Automatische Installation und Wartung jederzeit neu starten.</span><span class="sxs-lookup"><span data-stu-id="4ff27-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="4ff27-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="4ff27-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="4ff27-123">4</span><span class="sxs-lookup"><span data-stu-id="4ff27-123">4</span></span>|<span data-ttu-id="4ff27-124">Automatische Installation und zum geplanten Zeitpunkt neu starten.</span><span class="sxs-lookup"><span data-stu-id="4ff27-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="4ff27-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="4ff27-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="4ff27-126">5</span><span class="sxs-lookup"><span data-stu-id="4ff27-126">5</span></span>|<span data-ttu-id="4ff27-127">Automatische Installation und neu starten Sie, ohne Kontrolle durch den Endbenutzer</span><span class="sxs-lookup"><span data-stu-id="4ff27-127">Auto-install and restart without end-user control</span></span>|



