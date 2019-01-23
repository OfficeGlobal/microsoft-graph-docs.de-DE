---
title: ManagedAppDataEncryptionType Enum-Typ
description: Stellt die Ebene an die app-Daten für verwaltete apps verschlüsselt werden
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 00174e7fba8a8da7490d04815b07a794a966179c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413689"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="b2792-103">ManagedAppDataEncryptionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="b2792-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="b2792-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b2792-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b2792-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b2792-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b2792-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b2792-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2792-107">Stellt die Ebene an die app-Daten für verwaltete apps verschlüsselt werden</span><span class="sxs-lookup"><span data-stu-id="b2792-107">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="b2792-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="b2792-108">Members</span></span>
|<span data-ttu-id="b2792-109">Member</span><span class="sxs-lookup"><span data-stu-id="b2792-109">Member</span></span>|<span data-ttu-id="b2792-110">Wert</span><span class="sxs-lookup"><span data-stu-id="b2792-110">Value</span></span>|<span data-ttu-id="b2792-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2792-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2792-112">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="b2792-112">useDeviceSettings</span></span>|<span data-ttu-id="b2792-113">0</span><span class="sxs-lookup"><span data-stu-id="b2792-113">0</span></span>|<span data-ttu-id="b2792-114">App-Daten werden verschlüsselt basierend auf die Standardeinstellungen auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="b2792-114">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="b2792-115">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="b2792-115">afterDeviceRestart</span></span>|<span data-ttu-id="b2792-116">1</span><span class="sxs-lookup"><span data-stu-id="b2792-116">1</span></span>|<span data-ttu-id="b2792-117">App-Daten werden verschlüsselt, wenn das Gerät neu gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="b2792-117">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="b2792-118">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="b2792-118">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="b2792-119">2</span><span class="sxs-lookup"><span data-stu-id="b2792-119">2</span></span>|<span data-ttu-id="b2792-120">App-Daten, die diese Richtlinie zugeordnet werden verschlüsselt, wenn das Gerät, mit Ausnahme von Daten in Dateien gesperrt ist, die geöffnet sind</span><span class="sxs-lookup"><span data-stu-id="b2792-120">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="b2792-121">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="b2792-121">whenDeviceLocked</span></span>|<span data-ttu-id="b2792-122">3</span><span class="sxs-lookup"><span data-stu-id="b2792-122">3</span></span>|<span data-ttu-id="b2792-123">App-Daten, die diese Richtlinie zugeordnet werden verschlüsselt, wenn das Gerät gesperrt ist</span><span class="sxs-lookup"><span data-stu-id="b2792-123">App data associated with this policy is encrypted when the device is locked</span></span>|




