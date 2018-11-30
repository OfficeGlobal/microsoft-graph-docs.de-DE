---
title: ManagedAppDataEncryptionType Enum-Typ
description: Stellt die Ebene an die app-Daten für verwaltete apps verschlüsselt werden
ms.openlocfilehash: 7efda037bc2b4d5794c575823845c0955be46477
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018849"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="4a49f-103">ManagedAppDataEncryptionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="4a49f-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="4a49f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4a49f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a49f-105">Stellt die Ebene an die app-Daten für verwaltete apps verschlüsselt werden</span><span class="sxs-lookup"><span data-stu-id="4a49f-105">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="4a49f-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="4a49f-106">Members</span></span>
|<span data-ttu-id="4a49f-107">Element</span><span class="sxs-lookup"><span data-stu-id="4a49f-107">Member</span></span>|<span data-ttu-id="4a49f-108">Wert</span><span class="sxs-lookup"><span data-stu-id="4a49f-108">Value</span></span>|<span data-ttu-id="4a49f-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a49f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a49f-110">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="4a49f-110">useDeviceSettings</span></span>|<span data-ttu-id="4a49f-111">0</span><span class="sxs-lookup"><span data-stu-id="4a49f-111">0</span></span>|<span data-ttu-id="4a49f-112">App-Daten werden verschlüsselt basierend auf die Standardeinstellungen auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="4a49f-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="4a49f-113">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="4a49f-113">afterDeviceRestart</span></span>|<span data-ttu-id="4a49f-114">1</span><span class="sxs-lookup"><span data-stu-id="4a49f-114">1</span></span>|<span data-ttu-id="4a49f-115">App-Daten werden verschlüsselt, wenn das Gerät neu gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="4a49f-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="4a49f-116">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="4a49f-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="4a49f-117">2</span><span class="sxs-lookup"><span data-stu-id="4a49f-117">2</span></span>|<span data-ttu-id="4a49f-118">App-Daten, die diese Richtlinie zugeordnet werden verschlüsselt, wenn das Gerät, mit Ausnahme von Daten in Dateien gesperrt ist, die geöffnet sind</span><span class="sxs-lookup"><span data-stu-id="4a49f-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="4a49f-119">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="4a49f-119">whenDeviceLocked</span></span>|<span data-ttu-id="4a49f-120">3</span><span class="sxs-lookup"><span data-stu-id="4a49f-120">3</span></span>|<span data-ttu-id="4a49f-121">App-Daten, die diese Richtlinie zugeordnet werden verschlüsselt, wenn das Gerät gesperrt ist</span><span class="sxs-lookup"><span data-stu-id="4a49f-121">App data associated with this policy is encrypted when the device is locked</span></span>|


