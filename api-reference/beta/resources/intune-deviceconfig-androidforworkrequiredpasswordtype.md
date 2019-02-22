---
title: androidForWorkRequiredPasswordType-Enumerationstyp
description: Android for Work erforderlicher Kennworttyp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e0e99a5e54797441070308882d4137859390820
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169475"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="16ecf-103">androidForWorkRequiredPasswordType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="16ecf-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="16ecf-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16ecf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16ecf-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="16ecf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16ecf-106">Android for Work erforderlicher Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="16ecf-106">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="16ecf-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="16ecf-107">Members</span></span>
|<span data-ttu-id="16ecf-108">Element</span><span class="sxs-lookup"><span data-stu-id="16ecf-108">Member</span></span>|<span data-ttu-id="16ecf-109">Wert</span><span class="sxs-lookup"><span data-stu-id="16ecf-109">Value</span></span>|<span data-ttu-id="16ecf-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16ecf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16ecf-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="16ecf-111">deviceDefault</span></span>|<span data-ttu-id="16ecf-112">0</span><span class="sxs-lookup"><span data-stu-id="16ecf-112">0</span></span>|<span data-ttu-id="16ecf-113">Geräte-Standardwert, keine Absicht.</span><span class="sxs-lookup"><span data-stu-id="16ecf-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="16ecf-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="16ecf-114">lowSecurityBiometric</span></span>|<span data-ttu-id="16ecf-115">1</span><span class="sxs-lookup"><span data-stu-id="16ecf-115">1</span></span>|<span data-ttu-id="16ecf-116">Niedriges Biometrie-basiertes Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16ecf-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="16ecf-117">erforderlich</span><span class="sxs-lookup"><span data-stu-id="16ecf-117">required</span></span>|<span data-ttu-id="16ecf-118">2</span><span class="sxs-lookup"><span data-stu-id="16ecf-118">2</span></span>|<span data-ttu-id="16ecf-119">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16ecf-119">Required.</span></span>|
|<span data-ttu-id="16ecf-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="16ecf-120">atLeastNumeric</span></span>|<span data-ttu-id="16ecf-121">3</span><span class="sxs-lookup"><span data-stu-id="16ecf-121">3</span></span>|<span data-ttu-id="16ecf-122">Mindestens ein numerisches Kennwort ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16ecf-122">At least numeric password required.</span></span>|
|<span data-ttu-id="16ecf-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="16ecf-123">numericComplex</span></span>|<span data-ttu-id="16ecf-124">4</span><span class="sxs-lookup"><span data-stu-id="16ecf-124">4</span></span>|<span data-ttu-id="16ecf-125">Numerisches komplexes Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16ecf-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="16ecf-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="16ecf-126">atLeastAlphabetic</span></span>|<span data-ttu-id="16ecf-127">5</span><span class="sxs-lookup"><span data-stu-id="16ecf-127">5</span></span>|<span data-ttu-id="16ecf-128">Mindestens ein alphabetisches Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16ecf-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="16ecf-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="16ecf-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="16ecf-130">6</span><span class="sxs-lookup"><span data-stu-id="16ecf-130">6</span></span>|<span data-ttu-id="16ecf-131">Mindestens alphanumerisches Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16ecf-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="16ecf-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="16ecf-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="16ecf-133">7</span><span class="sxs-lookup"><span data-stu-id="16ecf-133">7</span></span>|<span data-ttu-id="16ecf-134">Mindestens alphanumerisch mit Symbol Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16ecf-134">At least alphanumeric with symbols password required.</span></span>|




