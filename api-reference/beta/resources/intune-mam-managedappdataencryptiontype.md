---
title: managedAppDataEncryptionType-Enumerationstyp
description: Stellt die Ebene dar, auf die APP-Daten für verwaltete apps verschlüsselt werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47396f32ed23234c5fe758a29b6e97ee3602234f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159080"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="feb78-103">managedAppDataEncryptionType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="feb78-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="feb78-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="feb78-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="feb78-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="feb78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="feb78-106">Stellt die Ebene dar, auf die APP-Daten für verwaltete apps verschlüsselt werden.</span><span class="sxs-lookup"><span data-stu-id="feb78-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="feb78-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="feb78-107">Members</span></span>
|<span data-ttu-id="feb78-108">Element</span><span class="sxs-lookup"><span data-stu-id="feb78-108">Member</span></span>|<span data-ttu-id="feb78-109">Wert</span><span class="sxs-lookup"><span data-stu-id="feb78-109">Value</span></span>|<span data-ttu-id="feb78-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="feb78-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="feb78-111">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="feb78-111">useDeviceSettings</span></span>|<span data-ttu-id="feb78-112">0</span><span class="sxs-lookup"><span data-stu-id="feb78-112">0</span></span>|<span data-ttu-id="feb78-113">App-Daten werden basierend auf den Standardeinstellungen auf dem Gerät verschlüsselt.</span><span class="sxs-lookup"><span data-stu-id="feb78-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="feb78-114">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="feb78-114">afterDeviceRestart</span></span>|<span data-ttu-id="feb78-115">1</span><span class="sxs-lookup"><span data-stu-id="feb78-115">1</span></span>|<span data-ttu-id="feb78-116">App-Daten werden beim Neustart des Geräts verschlüsselt.</span><span class="sxs-lookup"><span data-stu-id="feb78-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="feb78-117">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="feb78-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="feb78-118">2</span><span class="sxs-lookup"><span data-stu-id="feb78-118">2</span></span>|<span data-ttu-id="feb78-119">App-Daten, die dieser Richtlinie zugeordnet sind, werden verschlüsselt, wenn das Gerät gesperrt ist, mit Ausnahme von Daten in geöffneten Dateien</span><span class="sxs-lookup"><span data-stu-id="feb78-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="feb78-120">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="feb78-120">whenDeviceLocked</span></span>|<span data-ttu-id="feb78-121">3</span><span class="sxs-lookup"><span data-stu-id="feb78-121">3</span></span>|<span data-ttu-id="feb78-122">App-Daten, die dieser Richtlinie zugeordnet sind, werden verschlüsselt, wenn das Gerät gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="feb78-122">App data associated with this policy is encrypted when the device is locked</span></span>|




