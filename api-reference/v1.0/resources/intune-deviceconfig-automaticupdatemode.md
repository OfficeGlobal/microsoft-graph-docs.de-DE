---
title: Eigenschaften automaticupdatemode-Enumerationstyp
description: Mögliche Werte für den automatischen Aktualisierungsmodus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fd45ff85cbab934aa2549f13ee3e6671c65f9ae
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251377"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="65ec1-103">Eigenschaften automaticupdatemode-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="65ec1-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="65ec1-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="65ec1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65ec1-105">Mögliche Werte für den automatischen Aktualisierungsmodus.</span><span class="sxs-lookup"><span data-stu-id="65ec1-105">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="65ec1-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="65ec1-106">Members</span></span>
|<span data-ttu-id="65ec1-107">Element</span><span class="sxs-lookup"><span data-stu-id="65ec1-107">Member</span></span>|<span data-ttu-id="65ec1-108">Wert</span><span class="sxs-lookup"><span data-stu-id="65ec1-108">Value</span></span>|<span data-ttu-id="65ec1-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65ec1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65ec1-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="65ec1-110">userDefined</span></span>|<span data-ttu-id="65ec1-111">0</span><span class="sxs-lookup"><span data-stu-id="65ec1-111">0</span></span>|<span data-ttu-id="65ec1-112">Benutzerdefiniert, Standardwert, keine Absicht.</span><span class="sxs-lookup"><span data-stu-id="65ec1-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="65ec1-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="65ec1-113">notifyDownload</span></span>|<span data-ttu-id="65ec1-114">1</span><span class="sxs-lookup"><span data-stu-id="65ec1-114">1</span></span>|<span data-ttu-id="65ec1-115">Benachrichtigung beim Download.</span><span class="sxs-lookup"><span data-stu-id="65ec1-115">Notify on download.</span></span>|
|<span data-ttu-id="65ec1-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="65ec1-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="65ec1-117">2</span><span class="sxs-lookup"><span data-stu-id="65ec1-117">2</span></span>|<span data-ttu-id="65ec1-118">Automatische Installation zur Wartungszeit.</span><span class="sxs-lookup"><span data-stu-id="65ec1-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="65ec1-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="65ec1-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="65ec1-120">3</span><span class="sxs-lookup"><span data-stu-id="65ec1-120">3</span></span>|<span data-ttu-id="65ec1-121">Automatisches Installieren und Neustarten zum Zeitpunkt der Wartung.</span><span class="sxs-lookup"><span data-stu-id="65ec1-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="65ec1-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="65ec1-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="65ec1-123">4</span><span class="sxs-lookup"><span data-stu-id="65ec1-123">4</span></span>|<span data-ttu-id="65ec1-124">Automatisches Installieren und Neustarten zum geplanten Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="65ec1-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="65ec1-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="65ec1-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="65ec1-126">5</span><span class="sxs-lookup"><span data-stu-id="65ec1-126">5</span></span>|<span data-ttu-id="65ec1-127">Automatisches Installieren und Neustarten ohne Endbenutzer Steuerelement</span><span class="sxs-lookup"><span data-stu-id="65ec1-127">Auto-install and restart without end-user control</span></span>|



