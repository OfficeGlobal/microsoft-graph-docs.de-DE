---
title: deviceGuardLocalSystemAuthorityCredentialGuardType-Enumerationstyp
description: Mögliche Werte der Einstellungen für den Anmelde Informationenschutz.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8452f24f0bc5641d9d7ebcfd68c8cd593443554d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167858"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="b8145-103">deviceGuardLocalSystemAuthorityCredentialGuardType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="b8145-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="b8145-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8145-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8145-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b8145-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8145-106">Mögliche Werte der Einstellungen für den Anmelde Informationenschutz.</span><span class="sxs-lookup"><span data-stu-id="b8145-106">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="b8145-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="b8145-107">Members</span></span>
|<span data-ttu-id="b8145-108">Element</span><span class="sxs-lookup"><span data-stu-id="b8145-108">Member</span></span>|<span data-ttu-id="b8145-109">Wert</span><span class="sxs-lookup"><span data-stu-id="b8145-109">Value</span></span>|<span data-ttu-id="b8145-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8145-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8145-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b8145-111">notConfigured</span></span>|<span data-ttu-id="b8145-112">0</span><span class="sxs-lookup"><span data-stu-id="b8145-112">0</span></span>|<span data-ttu-id="b8145-113">Deaktiviert die Überwachung der Anmeldeinformationen, wenn Sie zuvor ohne UEFI-Sperre konfiguriert wurden.</span><span class="sxs-lookup"><span data-stu-id="b8145-113">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="b8145-114">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="b8145-114">enableWithUEFILock</span></span>|<span data-ttu-id="b8145-115">1</span><span class="sxs-lookup"><span data-stu-id="b8145-115">1</span></span>|<span data-ttu-id="b8145-116">Aktiviert den Schutz von Anmeldeinformationen mit UEFI-Sperre.</span><span class="sxs-lookup"><span data-stu-id="b8145-116">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="b8145-117">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="b8145-117">enableWithoutUEFILock</span></span>|<span data-ttu-id="b8145-118">2</span><span class="sxs-lookup"><span data-stu-id="b8145-118">2</span></span>|<span data-ttu-id="b8145-119">Aktiviert den Schutz von Anmeldeinformationen ohne UEFI-Sperre.</span><span class="sxs-lookup"><span data-stu-id="b8145-119">Turns on Credential Guard without UEFI lock.</span></span>|




