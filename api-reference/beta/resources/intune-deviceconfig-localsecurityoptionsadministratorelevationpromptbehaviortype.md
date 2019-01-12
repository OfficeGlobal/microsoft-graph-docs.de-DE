---
title: LocalSecurityOptionsAdministratorElevationPromptBehaviorType Enum-Typ
description: Mögliche Werte für LocalSecurityOptionsAdministratorElevationPromptBehavior
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ae886f6c7696150cb85a17cb2caa65823705e121
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916824"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="1c078-103">LocalSecurityOptionsAdministratorElevationPromptBehaviorType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="1c078-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="1c078-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1c078-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c078-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1c078-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c078-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1c078-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c078-107">Mögliche Werte für LocalSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="1c078-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>
## <a name="members"></a><span data-ttu-id="1c078-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="1c078-108">Members</span></span>
|<span data-ttu-id="1c078-109">Element</span><span class="sxs-lookup"><span data-stu-id="1c078-109">Member</span></span>|<span data-ttu-id="1c078-110">Wert</span><span class="sxs-lookup"><span data-stu-id="1c078-110">Value</span></span>|<span data-ttu-id="1c078-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c078-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c078-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="1c078-112">notConfigured</span></span>|<span data-ttu-id="1c078-113">0</span><span class="sxs-lookup"><span data-stu-id="1c078-113">0</span></span>|<span data-ttu-id="1c078-114">Nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="1c078-114">Not Configured</span></span>|
|<span data-ttu-id="1c078-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="1c078-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="1c078-116">1</span><span class="sxs-lookup"><span data-stu-id="1c078-116">1</span></span>|<span data-ttu-id="1c078-117">Zu erhöhen, ohne aufzufordern.</span><span class="sxs-lookup"><span data-stu-id="1c078-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="1c078-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="1c078-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="1c078-119">2</span><span class="sxs-lookup"><span data-stu-id="1c078-119">2</span></span>|<span data-ttu-id="1c078-120">Aufforderung zur erneuten Eingabe auf dem sicheren desktop</span><span class="sxs-lookup"><span data-stu-id="1c078-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="1c078-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="1c078-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="1c078-122">3</span><span class="sxs-lookup"><span data-stu-id="1c078-122">3</span></span>|<span data-ttu-id="1c078-123">Aufforderung zur Bestätigung auf dem sicheren desktop</span><span class="sxs-lookup"><span data-stu-id="1c078-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="1c078-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="1c078-124">promptForCredentials</span></span>|<span data-ttu-id="1c078-125">4</span><span class="sxs-lookup"><span data-stu-id="1c078-125">4</span></span>|<span data-ttu-id="1c078-126">Aufforderung zur erneuten Eingabe</span><span class="sxs-lookup"><span data-stu-id="1c078-126">Prompt for credentials</span></span>|
|<span data-ttu-id="1c078-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="1c078-127">promptForConsent</span></span>|<span data-ttu-id="1c078-128">5</span><span class="sxs-lookup"><span data-stu-id="1c078-128">5</span></span>|<span data-ttu-id="1c078-129">Aufforderung zur Bestätigung</span><span class="sxs-lookup"><span data-stu-id="1c078-129">Prompt for consent</span></span>|
|<span data-ttu-id="1c078-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="1c078-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="1c078-131">6</span><span class="sxs-lookup"><span data-stu-id="1c078-131">6</span></span>|<span data-ttu-id="1c078-132">Aufforderung zur Bestätigung für nicht-Windows-Binärdateien</span><span class="sxs-lookup"><span data-stu-id="1c078-132">Prompt for consent for non-Windows binaries</span></span>|





