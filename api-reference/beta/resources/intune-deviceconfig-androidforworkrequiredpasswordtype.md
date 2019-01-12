---
title: AndroidForWorkRequiredPasswordType Enum-Typ
description: Android für Arbeit erforderliche Kennworttyp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cc944cf87e9a8daa5c50f31fbb095f09dbee1a65
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933582"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="9a291-103">AndroidForWorkRequiredPasswordType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="9a291-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="9a291-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9a291-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a291-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9a291-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9a291-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9a291-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9a291-107">Android für Arbeit erforderliche Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="9a291-107">Android For Work required password type.</span></span>
## <a name="members"></a><span data-ttu-id="9a291-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="9a291-108">Members</span></span>
|<span data-ttu-id="9a291-109">Element</span><span class="sxs-lookup"><span data-stu-id="9a291-109">Member</span></span>|<span data-ttu-id="9a291-110">Wert</span><span class="sxs-lookup"><span data-stu-id="9a291-110">Value</span></span>|<span data-ttu-id="9a291-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9a291-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a291-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9a291-112">deviceDefault</span></span>|<span data-ttu-id="9a291-113">0</span><span class="sxs-lookup"><span data-stu-id="9a291-113">0</span></span>|<span data-ttu-id="9a291-114">Gerät Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="9a291-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="9a291-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="9a291-115">lowSecurityBiometric</span></span>|<span data-ttu-id="9a291-116">1</span><span class="sxs-lookup"><span data-stu-id="9a291-116">1</span></span>|<span data-ttu-id="9a291-117">Niedrige Sicherheit Biometrik basierend erforderliche Kennwort.</span><span class="sxs-lookup"><span data-stu-id="9a291-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="9a291-118">erforderlich</span><span class="sxs-lookup"><span data-stu-id="9a291-118">required</span></span>|<span data-ttu-id="9a291-119">2</span><span class="sxs-lookup"><span data-stu-id="9a291-119">2</span></span>|<span data-ttu-id="9a291-120">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9a291-120">Required.</span></span>|
|<span data-ttu-id="9a291-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="9a291-121">atLeastNumeric</span></span>|<span data-ttu-id="9a291-122">3</span><span class="sxs-lookup"><span data-stu-id="9a291-122">3</span></span>|<span data-ttu-id="9a291-123">Mindestens numerische erforderliche Kennwort.</span><span class="sxs-lookup"><span data-stu-id="9a291-123">At least numeric password required.</span></span>|
|<span data-ttu-id="9a291-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="9a291-124">numericComplex</span></span>|<span data-ttu-id="9a291-125">4</span><span class="sxs-lookup"><span data-stu-id="9a291-125">4</span></span>|<span data-ttu-id="9a291-126">Numerische komplexe Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9a291-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="9a291-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="9a291-127">atLeastAlphabetic</span></span>|<span data-ttu-id="9a291-128">5</span><span class="sxs-lookup"><span data-stu-id="9a291-128">5</span></span>|<span data-ttu-id="9a291-129">Mindestens alphabetische erforderliche Kennwort.</span><span class="sxs-lookup"><span data-stu-id="9a291-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="9a291-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="9a291-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="9a291-131">6</span><span class="sxs-lookup"><span data-stu-id="9a291-131">6</span></span>|<span data-ttu-id="9a291-132">Mindestens Alphanumerisches Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9a291-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="9a291-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="9a291-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="9a291-134">7</span><span class="sxs-lookup"><span data-stu-id="9a291-134">7</span></span>|<span data-ttu-id="9a291-135">Mindestens alphanumerisch Symbole erforderliche Kennwort.</span><span class="sxs-lookup"><span data-stu-id="9a291-135">At least alphanumeric with symbols password required.</span></span>|





