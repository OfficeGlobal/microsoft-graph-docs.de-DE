---
title: LocalSecurityOptionsAdministratorElevationPromptBehaviorType Enum-Typ
description: Mögliche Werte für LocalSecurityOptionsAdministratorElevationPromptBehavior
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 978436bca4ac0ca281fde61e046e854ba3725c73
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413759"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="04aa8-103">LocalSecurityOptionsAdministratorElevationPromptBehaviorType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="04aa8-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="04aa8-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="04aa8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="04aa8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="04aa8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04aa8-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="04aa8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04aa8-107">Mögliche Werte für LocalSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="04aa8-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="04aa8-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="04aa8-108">Members</span></span>
|<span data-ttu-id="04aa8-109">Member</span><span class="sxs-lookup"><span data-stu-id="04aa8-109">Member</span></span>|<span data-ttu-id="04aa8-110">Wert</span><span class="sxs-lookup"><span data-stu-id="04aa8-110">Value</span></span>|<span data-ttu-id="04aa8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04aa8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04aa8-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="04aa8-112">notConfigured</span></span>|<span data-ttu-id="04aa8-113">0</span><span class="sxs-lookup"><span data-stu-id="04aa8-113">0</span></span>|<span data-ttu-id="04aa8-114">Nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="04aa8-114">Not Configured</span></span>|
|<span data-ttu-id="04aa8-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="04aa8-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="04aa8-116">1</span><span class="sxs-lookup"><span data-stu-id="04aa8-116">1</span></span>|<span data-ttu-id="04aa8-117">Zu erhöhen, ohne aufzufordern.</span><span class="sxs-lookup"><span data-stu-id="04aa8-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="04aa8-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="04aa8-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="04aa8-119">2</span><span class="sxs-lookup"><span data-stu-id="04aa8-119">2</span></span>|<span data-ttu-id="04aa8-120">Aufforderung zur erneuten Eingabe auf dem sicheren desktop</span><span class="sxs-lookup"><span data-stu-id="04aa8-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="04aa8-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="04aa8-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="04aa8-122">3</span><span class="sxs-lookup"><span data-stu-id="04aa8-122">3</span></span>|<span data-ttu-id="04aa8-123">Aufforderung zur Bestätigung auf dem sicheren desktop</span><span class="sxs-lookup"><span data-stu-id="04aa8-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="04aa8-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="04aa8-124">promptForCredentials</span></span>|<span data-ttu-id="04aa8-125">4</span><span class="sxs-lookup"><span data-stu-id="04aa8-125">4</span></span>|<span data-ttu-id="04aa8-126">Aufforderung zur erneuten Eingabe</span><span class="sxs-lookup"><span data-stu-id="04aa8-126">Prompt for credentials</span></span>|
|<span data-ttu-id="04aa8-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="04aa8-127">promptForConsent</span></span>|<span data-ttu-id="04aa8-128">5</span><span class="sxs-lookup"><span data-stu-id="04aa8-128">5</span></span>|<span data-ttu-id="04aa8-129">Aufforderung zur Bestätigung</span><span class="sxs-lookup"><span data-stu-id="04aa8-129">Prompt for consent</span></span>|
|<span data-ttu-id="04aa8-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="04aa8-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="04aa8-131">6</span><span class="sxs-lookup"><span data-stu-id="04aa8-131">6</span></span>|<span data-ttu-id="04aa8-132">Aufforderung zur Bestätigung für nicht-Windows-Binärdateien</span><span class="sxs-lookup"><span data-stu-id="04aa8-132">Prompt for consent for non-Windows binaries</span></span>|




