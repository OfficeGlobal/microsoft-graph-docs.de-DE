---
title: managedAppDataEncryptionType-Enumerationstyp
description: Stellt die Ebene dar, auf die APP-Daten für verwaltete apps verschlüsselt werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 774312d5f19b223fd33e2c156610f516ae7f48a3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256770"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="a6983-103">managedAppDataEncryptionType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="a6983-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="a6983-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a6983-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6983-105">Stellt die Ebene dar, auf die APP-Daten für verwaltete apps verschlüsselt werden.</span><span class="sxs-lookup"><span data-stu-id="a6983-105">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="a6983-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="a6983-106">Members</span></span>
|<span data-ttu-id="a6983-107">Element</span><span class="sxs-lookup"><span data-stu-id="a6983-107">Member</span></span>|<span data-ttu-id="a6983-108">Wert</span><span class="sxs-lookup"><span data-stu-id="a6983-108">Value</span></span>|<span data-ttu-id="a6983-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a6983-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6983-110">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="a6983-110">useDeviceSettings</span></span>|<span data-ttu-id="a6983-111">0</span><span class="sxs-lookup"><span data-stu-id="a6983-111">0</span></span>|<span data-ttu-id="a6983-112">App-Daten werden basierend auf den Standardeinstellungen auf dem Gerät verschlüsselt.</span><span class="sxs-lookup"><span data-stu-id="a6983-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="a6983-113">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="a6983-113">afterDeviceRestart</span></span>|<span data-ttu-id="a6983-114">1</span><span class="sxs-lookup"><span data-stu-id="a6983-114">1</span></span>|<span data-ttu-id="a6983-115">App-Daten werden beim Neustart des Geräts verschlüsselt.</span><span class="sxs-lookup"><span data-stu-id="a6983-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="a6983-116">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="a6983-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="a6983-117">2</span><span class="sxs-lookup"><span data-stu-id="a6983-117">2</span></span>|<span data-ttu-id="a6983-118">App-Daten, die dieser Richtlinie zugeordnet sind, werden verschlüsselt, wenn das Gerät gesperrt ist, mit Ausnahme von Daten in geöffneten Dateien</span><span class="sxs-lookup"><span data-stu-id="a6983-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="a6983-119">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="a6983-119">whenDeviceLocked</span></span>|<span data-ttu-id="a6983-120">3</span><span class="sxs-lookup"><span data-stu-id="a6983-120">3</span></span>|<span data-ttu-id="a6983-121">App-Daten, die dieser Richtlinie zugeordnet sind, werden verschlüsselt, wenn das Gerät gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="a6983-121">App data associated with this policy is encrypted when the device is locked</span></span>|



