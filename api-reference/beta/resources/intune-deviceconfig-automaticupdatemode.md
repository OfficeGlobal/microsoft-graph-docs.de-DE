---
title: AutomaticUpdateMode Enum-Typ
description: Mögliche Werte für den Modus für automatische Updates.
ms.openlocfilehash: b7eac8337d6c8286e538bbe98b5ecbc13a448628
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063919"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="34705-103">AutomaticUpdateMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="34705-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="34705-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="34705-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34705-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34705-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34705-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="34705-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34705-107">Mögliche Werte für den Modus für automatische Updates.</span><span class="sxs-lookup"><span data-stu-id="34705-107">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="34705-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="34705-108">Members</span></span>
|<span data-ttu-id="34705-109">Element</span><span class="sxs-lookup"><span data-stu-id="34705-109">Member</span></span>|<span data-ttu-id="34705-110">Wert</span><span class="sxs-lookup"><span data-stu-id="34705-110">Value</span></span>|<span data-ttu-id="34705-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34705-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34705-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="34705-112">userDefined</span></span>|<span data-ttu-id="34705-113">0</span><span class="sxs-lookup"><span data-stu-id="34705-113">0</span></span>|<span data-ttu-id="34705-114">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="34705-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="34705-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="34705-115">notifyDownload</span></span>|<span data-ttu-id="34705-116">1</span><span class="sxs-lookup"><span data-stu-id="34705-116">1</span></span>|<span data-ttu-id="34705-117">Benachrichtigen Sie auf Download.</span><span class="sxs-lookup"><span data-stu-id="34705-117">Notify on download.</span></span>|
|<span data-ttu-id="34705-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="34705-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="34705-119">2</span><span class="sxs-lookup"><span data-stu-id="34705-119">2</span></span>|<span data-ttu-id="34705-120">Automatische Installation zur Wartungszeit.</span><span class="sxs-lookup"><span data-stu-id="34705-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="34705-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="34705-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="34705-122">3</span><span class="sxs-lookup"><span data-stu-id="34705-122">3</span></span>|<span data-ttu-id="34705-123">Automatische Installation und Wartung jederzeit neu starten.</span><span class="sxs-lookup"><span data-stu-id="34705-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="34705-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="34705-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="34705-125">4</span><span class="sxs-lookup"><span data-stu-id="34705-125">4</span></span>|<span data-ttu-id="34705-126">Automatische Installation und zum geplanten Zeitpunkt neu starten.</span><span class="sxs-lookup"><span data-stu-id="34705-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="34705-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="34705-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="34705-128">5</span><span class="sxs-lookup"><span data-stu-id="34705-128">5</span></span>|<span data-ttu-id="34705-129">Automatische Installation und neu starten Sie, ohne Kontrolle durch den Endbenutzer</span><span class="sxs-lookup"><span data-stu-id="34705-129">Auto-install and restart without end-user control</span></span>|





