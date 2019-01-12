---
title: AutomaticUpdateMode Enum-Typ
description: Mögliche Werte für den Modus für automatische Updates.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a31c50b5d16f4b9be8db4f95f2bbd9bd0ca123e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987860"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="63b96-103">AutomaticUpdateMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="63b96-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="63b96-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="63b96-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63b96-105">Mögliche Werte für den Modus für automatische Updates.</span><span class="sxs-lookup"><span data-stu-id="63b96-105">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="63b96-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="63b96-106">Members</span></span>
|<span data-ttu-id="63b96-107">Element</span><span class="sxs-lookup"><span data-stu-id="63b96-107">Member</span></span>|<span data-ttu-id="63b96-108">Wert</span><span class="sxs-lookup"><span data-stu-id="63b96-108">Value</span></span>|<span data-ttu-id="63b96-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63b96-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63b96-110">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="63b96-110">userDefined</span></span>|<span data-ttu-id="63b96-111">0</span><span class="sxs-lookup"><span data-stu-id="63b96-111">0</span></span>|<span data-ttu-id="63b96-112">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="63b96-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="63b96-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="63b96-113">notifyDownload</span></span>|<span data-ttu-id="63b96-114">1</span><span class="sxs-lookup"><span data-stu-id="63b96-114">1</span></span>|<span data-ttu-id="63b96-115">Benachrichtigen Sie auf Download.</span><span class="sxs-lookup"><span data-stu-id="63b96-115">Notify on download.</span></span>|
|<span data-ttu-id="63b96-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="63b96-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="63b96-117">2</span><span class="sxs-lookup"><span data-stu-id="63b96-117">2</span></span>|<span data-ttu-id="63b96-118">Automatische Installation zur Wartungszeit.</span><span class="sxs-lookup"><span data-stu-id="63b96-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="63b96-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="63b96-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="63b96-120">3</span><span class="sxs-lookup"><span data-stu-id="63b96-120">3</span></span>|<span data-ttu-id="63b96-121">Automatische Installation und Wartung jederzeit neu starten.</span><span class="sxs-lookup"><span data-stu-id="63b96-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="63b96-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="63b96-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="63b96-123">4</span><span class="sxs-lookup"><span data-stu-id="63b96-123">4</span></span>|<span data-ttu-id="63b96-124">Automatische Installation und zum geplanten Zeitpunkt neu starten.</span><span class="sxs-lookup"><span data-stu-id="63b96-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="63b96-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="63b96-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="63b96-126">5</span><span class="sxs-lookup"><span data-stu-id="63b96-126">5</span></span>|<span data-ttu-id="63b96-127">Automatische Installation und neu starten Sie, ohne Kontrolle durch den Endbenutzer</span><span class="sxs-lookup"><span data-stu-id="63b96-127">Auto-install and restart without end-user control</span></span>|



