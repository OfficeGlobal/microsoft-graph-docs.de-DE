---
title: AndroidWorkProfileRequiredPasswordType Enum-Typ
description: Android Arbeit Profil erforderliche Kennworttyp.
author: tfitzmac
ms.openlocfilehash: 8d41b4c516ee4aa393ea3a26034e5f575b58fa02
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330233"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="22132-103">AndroidWorkProfileRequiredPasswordType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="22132-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="22132-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="22132-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22132-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="22132-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22132-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="22132-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22132-107">Android Arbeit Profil erforderliche Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="22132-107">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="22132-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="22132-108">Members</span></span>
|<span data-ttu-id="22132-109">Member</span><span class="sxs-lookup"><span data-stu-id="22132-109">Member</span></span>|<span data-ttu-id="22132-110">Wert</span><span class="sxs-lookup"><span data-stu-id="22132-110">Value</span></span>|<span data-ttu-id="22132-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="22132-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22132-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="22132-112">deviceDefault</span></span>|<span data-ttu-id="22132-113">0</span><span class="sxs-lookup"><span data-stu-id="22132-113">0</span></span>|<span data-ttu-id="22132-114">Gerät Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="22132-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="22132-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="22132-115">lowSecurityBiometric</span></span>|<span data-ttu-id="22132-116">1</span><span class="sxs-lookup"><span data-stu-id="22132-116">1</span></span>|<span data-ttu-id="22132-117">Niedrige Sicherheit Biometrik basierend erforderliche Kennwort.</span><span class="sxs-lookup"><span data-stu-id="22132-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="22132-118">erforderlich</span><span class="sxs-lookup"><span data-stu-id="22132-118">required</span></span>|<span data-ttu-id="22132-119">2</span><span class="sxs-lookup"><span data-stu-id="22132-119">2</span></span>|<span data-ttu-id="22132-120">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="22132-120">Required.</span></span>|
|<span data-ttu-id="22132-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="22132-121">atLeastNumeric</span></span>|<span data-ttu-id="22132-122">3</span><span class="sxs-lookup"><span data-stu-id="22132-122">3</span></span>|<span data-ttu-id="22132-123">Mindestens numerische erforderliche Kennwort.</span><span class="sxs-lookup"><span data-stu-id="22132-123">At least numeric password required.</span></span>|
|<span data-ttu-id="22132-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="22132-124">numericComplex</span></span>|<span data-ttu-id="22132-125">4</span><span class="sxs-lookup"><span data-stu-id="22132-125">4</span></span>|<span data-ttu-id="22132-126">Numerische komplexe Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="22132-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="22132-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="22132-127">atLeastAlphabetic</span></span>|<span data-ttu-id="22132-128">5</span><span class="sxs-lookup"><span data-stu-id="22132-128">5</span></span>|<span data-ttu-id="22132-129">Mindestens alphabetische erforderliche Kennwort.</span><span class="sxs-lookup"><span data-stu-id="22132-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="22132-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="22132-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="22132-131">6</span><span class="sxs-lookup"><span data-stu-id="22132-131">6</span></span>|<span data-ttu-id="22132-132">Mindestens Alphanumerisches Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="22132-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="22132-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="22132-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="22132-134">7</span><span class="sxs-lookup"><span data-stu-id="22132-134">7</span></span>|<span data-ttu-id="22132-135">Mindestens alphanumerisch Symbole erforderliche Kennwort.</span><span class="sxs-lookup"><span data-stu-id="22132-135">At least alphanumeric with symbols password required.</span></span>|





