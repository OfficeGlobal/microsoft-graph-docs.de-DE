---
title: browserSyncSetting-Enumerationstyp
description: Die Synchronisierung der Einstellungen des Microsoft-Edge-Browsers zulassen (nicht konfiguriert) oder verhindern (blockieren). Option zum Verhindern der Synchronisierung über Geräte hinweg, aber Benutzer außer Kraft setzen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 71b5fd7addebdb24fce07644da9b33a2bb41f936
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152170"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="3939f-104">browserSyncSetting-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="3939f-104">browserSyncSetting enum type</span></span>

> <span data-ttu-id="3939f-105">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3939f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3939f-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3939f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3939f-107">Die Synchronisierung der Einstellungen des Microsoft-Edge-Browsers zulassen (nicht konfiguriert) oder verhindern (blockieren).</span><span class="sxs-lookup"><span data-stu-id="3939f-107">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="3939f-108">Option zum Verhindern der Synchronisierung über Geräte hinweg, aber Benutzer außer Kraft setzen.</span><span class="sxs-lookup"><span data-stu-id="3939f-108">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="3939f-109">Elemente</span><span class="sxs-lookup"><span data-stu-id="3939f-109">Members</span></span>
|<span data-ttu-id="3939f-110">Element</span><span class="sxs-lookup"><span data-stu-id="3939f-110">Member</span></span>|<span data-ttu-id="3939f-111">Wert</span><span class="sxs-lookup"><span data-stu-id="3939f-111">Value</span></span>|<span data-ttu-id="3939f-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3939f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3939f-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="3939f-113">notConfigured</span></span>|<span data-ttu-id="3939f-114">0</span><span class="sxs-lookup"><span data-stu-id="3939f-114">0</span></span>|<span data-ttu-id="3939f-115">Standard – ermöglicht die Synchronisierung von Browsereinstellungen auf Geräten.</span><span class="sxs-lookup"><span data-stu-id="3939f-115">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="3939f-116">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="3939f-116">blockedWithUserOverride</span></span>|<span data-ttu-id="3939f-117">1</span><span class="sxs-lookup"><span data-stu-id="3939f-117">1</span></span>|<span data-ttu-id="3939f-118">Verhindern der Synchronisierung von Browsereinstellungen über Benutzer Geräte hinweg, die Einstellung der Benutzer außer Kraft setzen.</span><span class="sxs-lookup"><span data-stu-id="3939f-118">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="3939f-119">gesperrt</span><span class="sxs-lookup"><span data-stu-id="3939f-119">blocked</span></span>|<span data-ttu-id="3939f-120">2</span><span class="sxs-lookup"><span data-stu-id="3939f-120">2</span></span>|<span data-ttu-id="3939f-121">Verhindern Sie die Synchronisierung von Browsereinstellungen auf Benutzergeräten.</span><span class="sxs-lookup"><span data-stu-id="3939f-121">Absolutely prevent syncing of browser settings across user devices.</span></span>|




