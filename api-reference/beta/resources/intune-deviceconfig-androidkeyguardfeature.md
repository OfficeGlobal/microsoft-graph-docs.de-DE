---
title: AndroidKeyguardFeature Enum-Typ
description: Android Keyguard Feature.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df89e1e9170bf2e3691116e27125514c7e0a6de9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430018"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="2a641-103">AndroidKeyguardFeature Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="2a641-103">androidKeyguardFeature enum type</span></span>

> <span data-ttu-id="2a641-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="2a641-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2a641-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a641-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2a641-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2a641-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a641-107">Android Keyguard Feature.</span><span class="sxs-lookup"><span data-stu-id="2a641-107">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="2a641-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="2a641-108">Members</span></span>
|<span data-ttu-id="2a641-109">Member</span><span class="sxs-lookup"><span data-stu-id="2a641-109">Member</span></span>|<span data-ttu-id="2a641-110">Wert</span><span class="sxs-lookup"><span data-stu-id="2a641-110">Value</span></span>|<span data-ttu-id="2a641-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a641-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a641-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="2a641-112">notConfigured</span></span>|<span data-ttu-id="2a641-113">0</span><span class="sxs-lookup"><span data-stu-id="2a641-113">0</span></span>|<span data-ttu-id="2a641-114">Nicht konfiguriert. Dieser Wert wird ignoriert.</span><span class="sxs-lookup"><span data-stu-id="2a641-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="2a641-115">Kamera</span><span class="sxs-lookup"><span data-stu-id="2a641-115">camera</span></span>|<span data-ttu-id="2a641-116">1</span><span class="sxs-lookup"><span data-stu-id="2a641-116">1</span></span>|<span data-ttu-id="2a641-117">Verwendung der Kamera beim auf sichere Keyguard Bildschirmen.</span><span class="sxs-lookup"><span data-stu-id="2a641-117">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="2a641-118">Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="2a641-118">notifications</span></span>|<span data-ttu-id="2a641-119">2</span><span class="sxs-lookup"><span data-stu-id="2a641-119">2</span></span>|<span data-ttu-id="2a641-120">Wenn auf sichere Keyguard Bildschirmen Benachrichtigungen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="2a641-120">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="2a641-121">unredactedNotifications</span><span class="sxs-lookup"><span data-stu-id="2a641-121">unredactedNotifications</span></span>|<span data-ttu-id="2a641-122">3</span><span class="sxs-lookup"><span data-stu-id="2a641-122">3</span></span>|<span data-ttu-id="2a641-123">Mit unredacted Benachrichtigungen, wenn auf sichere Keyguard Bildschirmen.</span><span class="sxs-lookup"><span data-stu-id="2a641-123">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="2a641-124">trustAgents</span><span class="sxs-lookup"><span data-stu-id="2a641-124">trustAgents</span></span>|<span data-ttu-id="2a641-125">4</span><span class="sxs-lookup"><span data-stu-id="2a641-125">4</span></span>|<span data-ttu-id="2a641-126">Wenn auf sichere Keyguard Bildschirmen Vertreterstatus vertrauen.</span><span class="sxs-lookup"><span data-stu-id="2a641-126">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="2a641-127">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="2a641-127">fingerprint</span></span>|<span data-ttu-id="2a641-128">5</span><span class="sxs-lookup"><span data-stu-id="2a641-128">5</span></span>|<span data-ttu-id="2a641-129">Fingerabdruck Sensor Usage beim auf sichere Keyguard Bildschirmen.</span><span class="sxs-lookup"><span data-stu-id="2a641-129">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="2a641-130">remoteInput</span><span class="sxs-lookup"><span data-stu-id="2a641-130">remoteInput</span></span>|<span data-ttu-id="2a641-131">6</span><span class="sxs-lookup"><span data-stu-id="2a641-131">6</span></span>|<span data-ttu-id="2a641-132">Benachrichtigung Texteingabe beim auf sichere Keyguard Bildschirmen.</span><span class="sxs-lookup"><span data-stu-id="2a641-132">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="2a641-133">allFeatures</span><span class="sxs-lookup"><span data-stu-id="2a641-133">allFeatures</span></span>|<span data-ttu-id="2a641-134">7</span><span class="sxs-lookup"><span data-stu-id="2a641-134">7</span></span>|<span data-ttu-id="2a641-135">Alle Keyguard Features beim auf sichere Keyguard Bildschirmen.</span><span class="sxs-lookup"><span data-stu-id="2a641-135">All keyguard features when on secure keyguard screens.</span></span>|




