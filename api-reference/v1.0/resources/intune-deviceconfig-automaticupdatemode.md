---
title: AutomaticUpdateMode Enum-Typ
description: Mögliche Werte für den Modus für automatische Updates.
author: tfitzmac
ms.openlocfilehash: 01e71e51a47a06aff12dd82e132d7eb468f26229
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346991"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="f7841-103">AutomaticUpdateMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="f7841-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="f7841-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f7841-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7841-105">Mögliche Werte für den Modus für automatische Updates.</span><span class="sxs-lookup"><span data-stu-id="f7841-105">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="f7841-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="f7841-106">Members</span></span>
|<span data-ttu-id="f7841-107">Member</span><span class="sxs-lookup"><span data-stu-id="f7841-107">Member</span></span>|<span data-ttu-id="f7841-108">Wert</span><span class="sxs-lookup"><span data-stu-id="f7841-108">Value</span></span>|<span data-ttu-id="f7841-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7841-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7841-110">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="f7841-110">userDefined</span></span>|<span data-ttu-id="f7841-111">0</span><span class="sxs-lookup"><span data-stu-id="f7841-111">0</span></span>|<span data-ttu-id="f7841-112">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="f7841-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="f7841-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="f7841-113">notifyDownload</span></span>|<span data-ttu-id="f7841-114">1</span><span class="sxs-lookup"><span data-stu-id="f7841-114">1</span></span>|<span data-ttu-id="f7841-115">Benachrichtigen Sie auf Download.</span><span class="sxs-lookup"><span data-stu-id="f7841-115">Notify on download.</span></span>|
|<span data-ttu-id="f7841-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="f7841-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="f7841-117">2</span><span class="sxs-lookup"><span data-stu-id="f7841-117">2</span></span>|<span data-ttu-id="f7841-118">Automatische Installation zur Wartungszeit.</span><span class="sxs-lookup"><span data-stu-id="f7841-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="f7841-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="f7841-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="f7841-120">3</span><span class="sxs-lookup"><span data-stu-id="f7841-120">3</span></span>|<span data-ttu-id="f7841-121">Automatische Installation und Wartung jederzeit neu starten.</span><span class="sxs-lookup"><span data-stu-id="f7841-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="f7841-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="f7841-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="f7841-123">4</span><span class="sxs-lookup"><span data-stu-id="f7841-123">4</span></span>|<span data-ttu-id="f7841-124">Automatische Installation und zum geplanten Zeitpunkt neu starten.</span><span class="sxs-lookup"><span data-stu-id="f7841-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="f7841-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="f7841-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="f7841-126">5</span><span class="sxs-lookup"><span data-stu-id="f7841-126">5</span></span>|<span data-ttu-id="f7841-127">Automatische Installation und neu starten Sie, ohne Kontrolle durch den Endbenutzer</span><span class="sxs-lookup"><span data-stu-id="f7841-127">Auto-install and restart without end-user control</span></span>|



