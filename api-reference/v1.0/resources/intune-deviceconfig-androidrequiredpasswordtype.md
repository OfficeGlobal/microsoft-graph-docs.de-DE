---
title: androidRequiredPasswordType-Enumerationstyp
description: Android erforderlicher Kennworttyp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59a95c74f19fa6e14440eaedd06d385b05d81e5d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255402"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="8f496-103">androidRequiredPasswordType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="8f496-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="8f496-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8f496-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f496-105">Android erforderlicher Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="8f496-105">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="8f496-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="8f496-106">Members</span></span>
|<span data-ttu-id="8f496-107">Element</span><span class="sxs-lookup"><span data-stu-id="8f496-107">Member</span></span>|<span data-ttu-id="8f496-108">Wert</span><span class="sxs-lookup"><span data-stu-id="8f496-108">Value</span></span>|<span data-ttu-id="8f496-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f496-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f496-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="8f496-110">deviceDefault</span></span>|<span data-ttu-id="8f496-111">0</span><span class="sxs-lookup"><span data-stu-id="8f496-111">0</span></span>|<span data-ttu-id="8f496-112">Geräte-Standardwert, keine Absicht.</span><span class="sxs-lookup"><span data-stu-id="8f496-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="8f496-113">alphabetischer</span><span class="sxs-lookup"><span data-stu-id="8f496-113">alphabetic</span></span>|<span data-ttu-id="8f496-114">1</span><span class="sxs-lookup"><span data-stu-id="8f496-114">1</span></span>|<span data-ttu-id="8f496-115">Alphabetisches Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8f496-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="8f496-116">Alphanumerisch</span><span class="sxs-lookup"><span data-stu-id="8f496-116">alphanumeric</span></span>|<span data-ttu-id="8f496-117">2</span><span class="sxs-lookup"><span data-stu-id="8f496-117">2</span></span>|<span data-ttu-id="8f496-118">Alphanumerisches Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8f496-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="8f496-119">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="8f496-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="8f496-120">3</span><span class="sxs-lookup"><span data-stu-id="8f496-120">3</span></span>|<span data-ttu-id="8f496-121">Alphanumerisch mit Symbol Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8f496-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="8f496-122">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="8f496-122">lowSecurityBiometric</span></span>|<span data-ttu-id="8f496-123">4</span><span class="sxs-lookup"><span data-stu-id="8f496-123">4</span></span>|<span data-ttu-id="8f496-124">Niedriges Biometrie-basiertes Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8f496-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="8f496-125">numerischen</span><span class="sxs-lookup"><span data-stu-id="8f496-125">numeric</span></span>|<span data-ttu-id="8f496-126">5</span><span class="sxs-lookup"><span data-stu-id="8f496-126">5</span></span>|<span data-ttu-id="8f496-127">Numerisches Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8f496-127">Numeric password required.</span></span>|
|<span data-ttu-id="8f496-128">numericComplex</span><span class="sxs-lookup"><span data-stu-id="8f496-128">numericComplex</span></span>|<span data-ttu-id="8f496-129">6</span><span class="sxs-lookup"><span data-stu-id="8f496-129">6</span></span>|<span data-ttu-id="8f496-130">Numerisches komplexes Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8f496-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="8f496-131">Beliebiger Wert</span><span class="sxs-lookup"><span data-stu-id="8f496-131">any</span></span>|<span data-ttu-id="8f496-132">7</span><span class="sxs-lookup"><span data-stu-id="8f496-132">7</span></span>|<span data-ttu-id="8f496-133">Ein Kennwort oder Muster ist erforderlich, und alle sind akzeptabel.</span><span class="sxs-lookup"><span data-stu-id="8f496-133">A password or pattern is required, and any is acceptable.</span></span>|



