---
title: androidWorkProfileRequiredPasswordType-Enumerationstyp
description: Android-Arbeitsprofil erforderlicher Kennworttyp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 742ffaff4c235f9abfeb44d707a3af4429fc86e6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169188"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="d3c1e-103">androidWorkProfileRequiredPasswordType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="d3c1e-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="d3c1e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d3c1e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3c1e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d3c1e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3c1e-106">Android-Arbeitsprofil erforderlicher Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="d3c1e-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="d3c1e-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="d3c1e-107">Members</span></span>
|<span data-ttu-id="d3c1e-108">Element</span><span class="sxs-lookup"><span data-stu-id="d3c1e-108">Member</span></span>|<span data-ttu-id="d3c1e-109">Wert</span><span class="sxs-lookup"><span data-stu-id="d3c1e-109">Value</span></span>|<span data-ttu-id="d3c1e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3c1e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3c1e-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d3c1e-111">deviceDefault</span></span>|<span data-ttu-id="d3c1e-112">0</span><span class="sxs-lookup"><span data-stu-id="d3c1e-112">0</span></span>|<span data-ttu-id="d3c1e-113">Geräte-Standardwert, keine Absicht.</span><span class="sxs-lookup"><span data-stu-id="d3c1e-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="d3c1e-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="d3c1e-114">lowSecurityBiometric</span></span>|<span data-ttu-id="d3c1e-115">1</span><span class="sxs-lookup"><span data-stu-id="d3c1e-115">1</span></span>|<span data-ttu-id="d3c1e-116">Niedriges Biometrie-basiertes Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d3c1e-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="d3c1e-117">erforderlich</span><span class="sxs-lookup"><span data-stu-id="d3c1e-117">required</span></span>|<span data-ttu-id="d3c1e-118">2</span><span class="sxs-lookup"><span data-stu-id="d3c1e-118">2</span></span>|<span data-ttu-id="d3c1e-119">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d3c1e-119">Required.</span></span>|
|<span data-ttu-id="d3c1e-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="d3c1e-120">atLeastNumeric</span></span>|<span data-ttu-id="d3c1e-121">3</span><span class="sxs-lookup"><span data-stu-id="d3c1e-121">3</span></span>|<span data-ttu-id="d3c1e-122">Mindestens ein numerisches Kennwort ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d3c1e-122">At least numeric password required.</span></span>|
|<span data-ttu-id="d3c1e-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="d3c1e-123">numericComplex</span></span>|<span data-ttu-id="d3c1e-124">4</span><span class="sxs-lookup"><span data-stu-id="d3c1e-124">4</span></span>|<span data-ttu-id="d3c1e-125">Numerisches komplexes Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d3c1e-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="d3c1e-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="d3c1e-126">atLeastAlphabetic</span></span>|<span data-ttu-id="d3c1e-127">5</span><span class="sxs-lookup"><span data-stu-id="d3c1e-127">5</span></span>|<span data-ttu-id="d3c1e-128">Mindestens ein alphabetisches Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d3c1e-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="d3c1e-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="d3c1e-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="d3c1e-130">6</span><span class="sxs-lookup"><span data-stu-id="d3c1e-130">6</span></span>|<span data-ttu-id="d3c1e-131">Mindestens alphanumerisches Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d3c1e-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="d3c1e-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="d3c1e-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="d3c1e-133">7</span><span class="sxs-lookup"><span data-stu-id="d3c1e-133">7</span></span>|<span data-ttu-id="d3c1e-134">Mindestens alphanumerisch mit Symbol Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d3c1e-134">At least alphanumeric with symbols password required.</span></span>|




