---
title: androidKeyguardFeature-Enumerationstyp
description: Android-Keyguard-Funktion.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2987a8220bbbcfc99238587a989b890aff958e47
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161950"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="3c872-103">androidKeyguardFeature-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="3c872-103">androidKeyguardFeature enum type</span></span>

> <span data-ttu-id="3c872-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c872-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c872-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3c872-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c872-106">Android-Keyguard-Funktion.</span><span class="sxs-lookup"><span data-stu-id="3c872-106">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="3c872-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="3c872-107">Members</span></span>
|<span data-ttu-id="3c872-108">Element</span><span class="sxs-lookup"><span data-stu-id="3c872-108">Member</span></span>|<span data-ttu-id="3c872-109">Wert</span><span class="sxs-lookup"><span data-stu-id="3c872-109">Value</span></span>|<span data-ttu-id="3c872-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c872-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c872-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="3c872-111">notConfigured</span></span>|<span data-ttu-id="3c872-112">0</span><span class="sxs-lookup"><span data-stu-id="3c872-112">0</span></span>|<span data-ttu-id="3c872-113">Nicht konfiguriert; Dieser Wert wird ignoriert.</span><span class="sxs-lookup"><span data-stu-id="3c872-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="3c872-114">Kamera</span><span class="sxs-lookup"><span data-stu-id="3c872-114">camera</span></span>|<span data-ttu-id="3c872-115">1</span><span class="sxs-lookup"><span data-stu-id="3c872-115">1</span></span>|<span data-ttu-id="3c872-116">Kamera Verwendung bei sicheren Bildschirmen.</span><span class="sxs-lookup"><span data-stu-id="3c872-116">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="3c872-117">Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="3c872-117">notifications</span></span>|<span data-ttu-id="3c872-118">2</span><span class="sxs-lookup"><span data-stu-id="3c872-118">2</span></span>|<span data-ttu-id="3c872-119">Anzeigen von Benachrichtigungen, wenn auf sicheren Keyguard-Bildschirmen.</span><span class="sxs-lookup"><span data-stu-id="3c872-119">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="3c872-120">unredactedNotifications</span><span class="sxs-lookup"><span data-stu-id="3c872-120">unredactedNotifications</span></span>|<span data-ttu-id="3c872-121">3</span><span class="sxs-lookup"><span data-stu-id="3c872-121">3</span></span>|<span data-ttu-id="3c872-122">Anzeigen von unzensierte-Benachrichtigungen, wenn auf sicheren Keyguard-Bildschirmen.</span><span class="sxs-lookup"><span data-stu-id="3c872-122">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="3c872-123">trustAgents</span><span class="sxs-lookup"><span data-stu-id="3c872-123">trustAgents</span></span>|<span data-ttu-id="3c872-124">4</span><span class="sxs-lookup"><span data-stu-id="3c872-124">4</span></span>|<span data-ttu-id="3c872-125">Trust-Agentstatus bei sicheren Bildschirmen.</span><span class="sxs-lookup"><span data-stu-id="3c872-125">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="3c872-126">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="3c872-126">fingerprint</span></span>|<span data-ttu-id="3c872-127">5</span><span class="sxs-lookup"><span data-stu-id="3c872-127">5</span></span>|<span data-ttu-id="3c872-128">Verwendung von Fingerabdrucksensoren bei Secure Keyguard-Bildschirmen.</span><span class="sxs-lookup"><span data-stu-id="3c872-128">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="3c872-129">remoteInput</span><span class="sxs-lookup"><span data-stu-id="3c872-129">remoteInput</span></span>|<span data-ttu-id="3c872-130">6</span><span class="sxs-lookup"><span data-stu-id="3c872-130">6</span></span>|<span data-ttu-id="3c872-131">Benachrichtigungstext Eintrag bei Secure Keyguard-Bildschirmen.</span><span class="sxs-lookup"><span data-stu-id="3c872-131">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="3c872-132">allFeatures</span><span class="sxs-lookup"><span data-stu-id="3c872-132">allFeatures</span></span>|<span data-ttu-id="3c872-133">7</span><span class="sxs-lookup"><span data-stu-id="3c872-133">7</span></span>|<span data-ttu-id="3c872-134">Alle Keyguard-Features, wenn Sie auf sicheren Keyguard-Bildschirmen.</span><span class="sxs-lookup"><span data-stu-id="3c872-134">All keyguard features when on secure keyguard screens.</span></span>|




