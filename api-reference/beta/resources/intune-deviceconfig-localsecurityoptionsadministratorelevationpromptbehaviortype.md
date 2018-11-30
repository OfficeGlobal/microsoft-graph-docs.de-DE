---
title: LocalSecurityOptionsAdministratorElevationPromptBehaviorType Enum-Typ
description: Mögliche Werte für LocalSecurityOptionsAdministratorElevationPromptBehavior
ms.openlocfilehash: 2959aebbb12bc567427c8a9b06a5ce2380933241
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061597"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="b3aad-103">LocalSecurityOptionsAdministratorElevationPromptBehaviorType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="b3aad-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="b3aad-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b3aad-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3aad-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b3aad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3aad-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b3aad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3aad-107">Mögliche Werte für LocalSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="b3aad-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>
## <a name="members"></a><span data-ttu-id="b3aad-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="b3aad-108">Members</span></span>
|<span data-ttu-id="b3aad-109">Element</span><span class="sxs-lookup"><span data-stu-id="b3aad-109">Member</span></span>|<span data-ttu-id="b3aad-110">Wert</span><span class="sxs-lookup"><span data-stu-id="b3aad-110">Value</span></span>|<span data-ttu-id="b3aad-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3aad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3aad-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="b3aad-112">notConfigured</span></span>|<span data-ttu-id="b3aad-113">0</span><span class="sxs-lookup"><span data-stu-id="b3aad-113">0</span></span>|<span data-ttu-id="b3aad-114">Nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="b3aad-114">Not Configured</span></span>|
|<span data-ttu-id="b3aad-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="b3aad-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="b3aad-116">1</span><span class="sxs-lookup"><span data-stu-id="b3aad-116">1</span></span>|<span data-ttu-id="b3aad-117">Zu erhöhen, ohne aufzufordern.</span><span class="sxs-lookup"><span data-stu-id="b3aad-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="b3aad-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="b3aad-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="b3aad-119">2</span><span class="sxs-lookup"><span data-stu-id="b3aad-119">2</span></span>|<span data-ttu-id="b3aad-120">Aufforderung zur erneuten Eingabe auf dem sicheren desktop</span><span class="sxs-lookup"><span data-stu-id="b3aad-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="b3aad-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="b3aad-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="b3aad-122">3</span><span class="sxs-lookup"><span data-stu-id="b3aad-122">3</span></span>|<span data-ttu-id="b3aad-123">Aufforderung zur Bestätigung auf dem sicheren desktop</span><span class="sxs-lookup"><span data-stu-id="b3aad-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="b3aad-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="b3aad-124">promptForCredentials</span></span>|<span data-ttu-id="b3aad-125">4</span><span class="sxs-lookup"><span data-stu-id="b3aad-125">4</span></span>|<span data-ttu-id="b3aad-126">Aufforderung zur erneuten Eingabe</span><span class="sxs-lookup"><span data-stu-id="b3aad-126">Prompt for credentials</span></span>|
|<span data-ttu-id="b3aad-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="b3aad-127">promptForConsent</span></span>|<span data-ttu-id="b3aad-128">5</span><span class="sxs-lookup"><span data-stu-id="b3aad-128">5</span></span>|<span data-ttu-id="b3aad-129">Aufforderung zur Bestätigung</span><span class="sxs-lookup"><span data-stu-id="b3aad-129">Prompt for consent</span></span>|
|<span data-ttu-id="b3aad-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="b3aad-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="b3aad-131">6</span><span class="sxs-lookup"><span data-stu-id="b3aad-131">6</span></span>|<span data-ttu-id="b3aad-132">Aufforderung zur Bestätigung für nicht-Windows-Binärdateien</span><span class="sxs-lookup"><span data-stu-id="b3aad-132">Prompt for consent for non-Windows binaries</span></span>|





