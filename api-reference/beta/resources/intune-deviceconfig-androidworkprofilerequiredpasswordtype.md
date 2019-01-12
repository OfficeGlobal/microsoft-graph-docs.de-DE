---
title: AndroidWorkProfileRequiredPasswordType Enum-Typ
description: Android Arbeit Profil erforderliche Kennworttyp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 97820113cda826a97d5bac5854577d4b4434eb57
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912232"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="a7e48-103">AndroidWorkProfileRequiredPasswordType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="a7e48-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="a7e48-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a7e48-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7e48-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a7e48-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7e48-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a7e48-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7e48-107">Android Arbeit Profil erforderliche Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="a7e48-107">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="a7e48-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="a7e48-108">Members</span></span>
|<span data-ttu-id="a7e48-109">Element</span><span class="sxs-lookup"><span data-stu-id="a7e48-109">Member</span></span>|<span data-ttu-id="a7e48-110">Wert</span><span class="sxs-lookup"><span data-stu-id="a7e48-110">Value</span></span>|<span data-ttu-id="a7e48-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a7e48-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7e48-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a7e48-112">deviceDefault</span></span>|<span data-ttu-id="a7e48-113">0</span><span class="sxs-lookup"><span data-stu-id="a7e48-113">0</span></span>|<span data-ttu-id="a7e48-114">Gerät Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="a7e48-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="a7e48-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="a7e48-115">lowSecurityBiometric</span></span>|<span data-ttu-id="a7e48-116">1</span><span class="sxs-lookup"><span data-stu-id="a7e48-116">1</span></span>|<span data-ttu-id="a7e48-117">Niedrige Sicherheit Biometrik basierend erforderliche Kennwort.</span><span class="sxs-lookup"><span data-stu-id="a7e48-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="a7e48-118">erforderlich</span><span class="sxs-lookup"><span data-stu-id="a7e48-118">required</span></span>|<span data-ttu-id="a7e48-119">2</span><span class="sxs-lookup"><span data-stu-id="a7e48-119">2</span></span>|<span data-ttu-id="a7e48-120">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a7e48-120">Required.</span></span>|
|<span data-ttu-id="a7e48-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="a7e48-121">atLeastNumeric</span></span>|<span data-ttu-id="a7e48-122">3</span><span class="sxs-lookup"><span data-stu-id="a7e48-122">3</span></span>|<span data-ttu-id="a7e48-123">Mindestens numerische erforderliche Kennwort.</span><span class="sxs-lookup"><span data-stu-id="a7e48-123">At least numeric password required.</span></span>|
|<span data-ttu-id="a7e48-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="a7e48-124">numericComplex</span></span>|<span data-ttu-id="a7e48-125">4</span><span class="sxs-lookup"><span data-stu-id="a7e48-125">4</span></span>|<span data-ttu-id="a7e48-126">Numerische komplexe Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a7e48-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="a7e48-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="a7e48-127">atLeastAlphabetic</span></span>|<span data-ttu-id="a7e48-128">5</span><span class="sxs-lookup"><span data-stu-id="a7e48-128">5</span></span>|<span data-ttu-id="a7e48-129">Mindestens alphabetische erforderliche Kennwort.</span><span class="sxs-lookup"><span data-stu-id="a7e48-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="a7e48-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="a7e48-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="a7e48-131">6</span><span class="sxs-lookup"><span data-stu-id="a7e48-131">6</span></span>|<span data-ttu-id="a7e48-132">Mindestens Alphanumerisches Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a7e48-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="a7e48-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="a7e48-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="a7e48-134">7</span><span class="sxs-lookup"><span data-stu-id="a7e48-134">7</span></span>|<span data-ttu-id="a7e48-135">Mindestens alphanumerisch Symbole erforderliche Kennwort.</span><span class="sxs-lookup"><span data-stu-id="a7e48-135">At least alphanumeric with symbols password required.</span></span>|





