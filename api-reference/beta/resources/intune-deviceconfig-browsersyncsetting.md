---
title: BrowserSyncSetting Enum-Typ
description: Allow(Not Configured) oder prevent(Block) der Synchronisierung von Microsoft Edge Browsereinstellungen. Option, um zu verhindern, dass die Synchronisierung für Geräte, Benutzer außer Kraft setzen, aber zulassen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8dce2b82b1eea5e4b06ed0f6949ba6a403b073a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431500"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="ff0e2-104">BrowserSyncSetting Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="ff0e2-104">browserSyncSetting enum type</span></span>

> <span data-ttu-id="ff0e2-105">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ff0e2-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ff0e2-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff0e2-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff0e2-107">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ff0e2-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff0e2-108">Allow(Not Configured) oder prevent(Block) der Synchronisierung von Microsoft Edge Browsereinstellungen.</span><span class="sxs-lookup"><span data-stu-id="ff0e2-108">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="ff0e2-109">Option, um zu verhindern, dass die Synchronisierung für Geräte, Benutzer außer Kraft setzen, aber zulassen.</span><span class="sxs-lookup"><span data-stu-id="ff0e2-109">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="ff0e2-110">Elemente</span><span class="sxs-lookup"><span data-stu-id="ff0e2-110">Members</span></span>
|<span data-ttu-id="ff0e2-111">Member</span><span class="sxs-lookup"><span data-stu-id="ff0e2-111">Member</span></span>|<span data-ttu-id="ff0e2-112">Wert</span><span class="sxs-lookup"><span data-stu-id="ff0e2-112">Value</span></span>|<span data-ttu-id="ff0e2-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff0e2-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff0e2-114">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="ff0e2-114">notConfigured</span></span>|<span data-ttu-id="ff0e2-115">0</span><span class="sxs-lookup"><span data-stu-id="ff0e2-115">0</span></span>|<span data-ttu-id="ff0e2-116">Standard – Synchronisierung von Browsereinstellungen für Geräte zulassen.</span><span class="sxs-lookup"><span data-stu-id="ff0e2-116">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="ff0e2-117">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="ff0e2-117">blockedWithUserOverride</span></span>|<span data-ttu-id="ff0e2-118">1</span><span class="sxs-lookup"><span data-stu-id="ff0e2-118">1</span></span>|<span data-ttu-id="ff0e2-119">Synchronisieren von Browsereinstellungen für Benutzer Geräte zu verhindern, Überschreiben der Einstellung Benutzer zulassen.</span><span class="sxs-lookup"><span data-stu-id="ff0e2-119">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="ff0e2-120">gesperrt</span><span class="sxs-lookup"><span data-stu-id="ff0e2-120">blocked</span></span>|<span data-ttu-id="ff0e2-121">2</span><span class="sxs-lookup"><span data-stu-id="ff0e2-121">2</span></span>|<span data-ttu-id="ff0e2-122">Absolut zu verhindern, dass die Synchronisierung von Browsereinstellungen für Benutzer Geräte.</span><span class="sxs-lookup"><span data-stu-id="ff0e2-122">Absolutely prevent syncing of browser settings across user devices.</span></span>|




