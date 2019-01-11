---
title: AutomaticUpdateMode Enum-Typ
description: Mögliche Werte für den Modus für automatische Updates.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 08389dca4379b6fc0222068545ebb9bed250ba94
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863413"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="7575f-103">AutomaticUpdateMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="7575f-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="7575f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7575f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7575f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7575f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7575f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7575f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7575f-107">Mögliche Werte für den Modus für automatische Updates.</span><span class="sxs-lookup"><span data-stu-id="7575f-107">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="7575f-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="7575f-108">Members</span></span>
|<span data-ttu-id="7575f-109">Element</span><span class="sxs-lookup"><span data-stu-id="7575f-109">Member</span></span>|<span data-ttu-id="7575f-110">Wert</span><span class="sxs-lookup"><span data-stu-id="7575f-110">Value</span></span>|<span data-ttu-id="7575f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7575f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7575f-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="7575f-112">userDefined</span></span>|<span data-ttu-id="7575f-113">0</span><span class="sxs-lookup"><span data-stu-id="7575f-113">0</span></span>|<span data-ttu-id="7575f-114">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="7575f-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="7575f-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="7575f-115">notifyDownload</span></span>|<span data-ttu-id="7575f-116">1</span><span class="sxs-lookup"><span data-stu-id="7575f-116">1</span></span>|<span data-ttu-id="7575f-117">Benachrichtigen Sie auf Download.</span><span class="sxs-lookup"><span data-stu-id="7575f-117">Notify on download.</span></span>|
|<span data-ttu-id="7575f-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="7575f-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="7575f-119">2</span><span class="sxs-lookup"><span data-stu-id="7575f-119">2</span></span>|<span data-ttu-id="7575f-120">Automatische Installation zur Wartungszeit.</span><span class="sxs-lookup"><span data-stu-id="7575f-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="7575f-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="7575f-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="7575f-122">3</span><span class="sxs-lookup"><span data-stu-id="7575f-122">3</span></span>|<span data-ttu-id="7575f-123">Automatische Installation und Wartung jederzeit neu starten.</span><span class="sxs-lookup"><span data-stu-id="7575f-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="7575f-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="7575f-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="7575f-125">4</span><span class="sxs-lookup"><span data-stu-id="7575f-125">4</span></span>|<span data-ttu-id="7575f-126">Automatische Installation und zum geplanten Zeitpunkt neu starten.</span><span class="sxs-lookup"><span data-stu-id="7575f-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="7575f-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="7575f-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="7575f-128">5</span><span class="sxs-lookup"><span data-stu-id="7575f-128">5</span></span>|<span data-ttu-id="7575f-129">Automatische Installation und neu starten Sie, ohne Kontrolle durch den Endbenutzer</span><span class="sxs-lookup"><span data-stu-id="7575f-129">Auto-install and restart without end-user control</span></span>|





