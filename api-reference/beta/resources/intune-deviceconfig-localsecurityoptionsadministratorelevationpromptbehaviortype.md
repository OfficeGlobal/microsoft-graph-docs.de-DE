---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType-Enumerationstyp
description: Mögliche Werte für LocalSecurityOptionsAdministratorElevationPromptBehavior
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5deaccdd8e1f3707617fe2df06a5fec087a47625
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139340"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="f8bd6-103">localSecurityOptionsAdministratorElevationPromptBehaviorType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="f8bd6-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="f8bd6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f8bd6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8bd6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f8bd6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8bd6-106">Mögliche Werte für LocalSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="f8bd6-106">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="f8bd6-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="f8bd6-107">Members</span></span>
|<span data-ttu-id="f8bd6-108">Element</span><span class="sxs-lookup"><span data-stu-id="f8bd6-108">Member</span></span>|<span data-ttu-id="f8bd6-109">Wert</span><span class="sxs-lookup"><span data-stu-id="f8bd6-109">Value</span></span>|<span data-ttu-id="f8bd6-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8bd6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8bd6-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f8bd6-111">notConfigured</span></span>|<span data-ttu-id="f8bd6-112">0</span><span class="sxs-lookup"><span data-stu-id="f8bd6-112">0</span></span>|<span data-ttu-id="f8bd6-113">Nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="f8bd6-113">Not Configured</span></span>|
|<span data-ttu-id="f8bd6-114">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="f8bd6-114">elevateWithoutPrompting</span></span>|<span data-ttu-id="f8bd6-115">1</span><span class="sxs-lookup"><span data-stu-id="f8bd6-115">1</span></span>|<span data-ttu-id="f8bd6-116">Ohne Ansagen erhöhen.</span><span class="sxs-lookup"><span data-stu-id="f8bd6-116">Elevate without prompting.</span></span>|
|<span data-ttu-id="f8bd6-117">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="f8bd6-117">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="f8bd6-118">2</span><span class="sxs-lookup"><span data-stu-id="f8bd6-118">2</span></span>|<span data-ttu-id="f8bd6-119">Anfordern von Anmeldeinformationen auf dem sicheren Desktop</span><span class="sxs-lookup"><span data-stu-id="f8bd6-119">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="f8bd6-120">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="f8bd6-120">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="f8bd6-121">3</span><span class="sxs-lookup"><span data-stu-id="f8bd6-121">3</span></span>|<span data-ttu-id="f8bd6-122">Anfordern der Zustimmung auf dem sicheren Desktop</span><span class="sxs-lookup"><span data-stu-id="f8bd6-122">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="f8bd6-123">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="f8bd6-123">promptForCredentials</span></span>|<span data-ttu-id="f8bd6-124">4</span><span class="sxs-lookup"><span data-stu-id="f8bd6-124">4</span></span>|<span data-ttu-id="f8bd6-125">Anfordern von Anmeldeinformationen</span><span class="sxs-lookup"><span data-stu-id="f8bd6-125">Prompt for credentials</span></span>|
|<span data-ttu-id="f8bd6-126">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="f8bd6-126">promptForConsent</span></span>|<span data-ttu-id="f8bd6-127">5</span><span class="sxs-lookup"><span data-stu-id="f8bd6-127">5</span></span>|<span data-ttu-id="f8bd6-128">Bestätigung anfordern</span><span class="sxs-lookup"><span data-stu-id="f8bd6-128">Prompt for consent</span></span>|
|<span data-ttu-id="f8bd6-129">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="f8bd6-129">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="f8bd6-130">6</span><span class="sxs-lookup"><span data-stu-id="f8bd6-130">6</span></span>|<span data-ttu-id="f8bd6-131">Anfordern der Zustimmung für nicht-Windows-Binärdateien</span><span class="sxs-lookup"><span data-stu-id="f8bd6-131">Prompt for consent for non-Windows binaries</span></span>|




