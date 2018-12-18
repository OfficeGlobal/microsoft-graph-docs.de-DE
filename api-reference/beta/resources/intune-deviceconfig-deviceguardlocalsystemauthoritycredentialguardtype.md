---
title: DeviceGuardLocalSystemAuthorityCredentialGuardType Enum-Typ
description: Mögliche Werte von Anmeldeinformationen Guard-Einstellungen.
author: tfitzmac
ms.openlocfilehash: 6f6c952d1c480d42db45de6345eba883ff5848a8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346963"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="fdf24-103">DeviceGuardLocalSystemAuthorityCredentialGuardType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="fdf24-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="fdf24-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fdf24-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fdf24-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fdf24-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fdf24-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fdf24-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fdf24-107">Mögliche Werte von Anmeldeinformationen Guard-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="fdf24-107">Possible values of Credential Guard settings.</span></span>
## <a name="members"></a><span data-ttu-id="fdf24-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="fdf24-108">Members</span></span>
|<span data-ttu-id="fdf24-109">Member</span><span class="sxs-lookup"><span data-stu-id="fdf24-109">Member</span></span>|<span data-ttu-id="fdf24-110">Wert</span><span class="sxs-lookup"><span data-stu-id="fdf24-110">Value</span></span>|<span data-ttu-id="fdf24-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdf24-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdf24-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="fdf24-112">notConfigured</span></span>|<span data-ttu-id="fdf24-113">0</span><span class="sxs-lookup"><span data-stu-id="fdf24-113">0</span></span>|<span data-ttu-id="fdf24-114">Schaltet Anmeldeinformationen Guard Remote Wenn zuvor ohne UEFI Sperre konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="fdf24-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="fdf24-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="fdf24-115">enableWithUEFILock</span></span>|<span data-ttu-id="fdf24-116">1</span><span class="sxs-lookup"><span data-stu-id="fdf24-116">1</span></span>|<span data-ttu-id="fdf24-117">Aktiviert die Anmeldeinformationen Guard mit UEFI sperren.</span><span class="sxs-lookup"><span data-stu-id="fdf24-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="fdf24-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="fdf24-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="fdf24-119">2</span><span class="sxs-lookup"><span data-stu-id="fdf24-119">2</span></span>|<span data-ttu-id="fdf24-120">Aktiviert die Anmeldeinformationen Guard ohne UEFI sperren.</span><span class="sxs-lookup"><span data-stu-id="fdf24-120">Turns on Credential Guard without UEFI lock.</span></span>|





