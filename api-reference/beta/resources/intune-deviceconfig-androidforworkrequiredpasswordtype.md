---
title: AndroidForWorkRequiredPasswordType Enum-Typ
description: Android für Arbeit erforderliche Kennworttyp.
author: tfitzmac
ms.openlocfilehash: cefb41dea7a92f1b1a640d8c9bf701a321ad9ead
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357281"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="487df-103">AndroidForWorkRequiredPasswordType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="487df-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="487df-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="487df-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="487df-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="487df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="487df-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="487df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="487df-107">Android für Arbeit erforderliche Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="487df-107">Android For Work required password type.</span></span>
## <a name="members"></a><span data-ttu-id="487df-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="487df-108">Members</span></span>
|<span data-ttu-id="487df-109">Member</span><span class="sxs-lookup"><span data-stu-id="487df-109">Member</span></span>|<span data-ttu-id="487df-110">Wert</span><span class="sxs-lookup"><span data-stu-id="487df-110">Value</span></span>|<span data-ttu-id="487df-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="487df-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="487df-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="487df-112">deviceDefault</span></span>|<span data-ttu-id="487df-113">0</span><span class="sxs-lookup"><span data-stu-id="487df-113">0</span></span>|<span data-ttu-id="487df-114">Gerät Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="487df-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="487df-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="487df-115">lowSecurityBiometric</span></span>|<span data-ttu-id="487df-116">1</span><span class="sxs-lookup"><span data-stu-id="487df-116">1</span></span>|<span data-ttu-id="487df-117">Niedrige Sicherheit Biometrik basierend erforderliche Kennwort.</span><span class="sxs-lookup"><span data-stu-id="487df-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="487df-118">erforderlich</span><span class="sxs-lookup"><span data-stu-id="487df-118">required</span></span>|<span data-ttu-id="487df-119">2</span><span class="sxs-lookup"><span data-stu-id="487df-119">2</span></span>|<span data-ttu-id="487df-120">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="487df-120">Required.</span></span>|
|<span data-ttu-id="487df-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="487df-121">atLeastNumeric</span></span>|<span data-ttu-id="487df-122">3</span><span class="sxs-lookup"><span data-stu-id="487df-122">3</span></span>|<span data-ttu-id="487df-123">Mindestens numerische erforderliche Kennwort.</span><span class="sxs-lookup"><span data-stu-id="487df-123">At least numeric password required.</span></span>|
|<span data-ttu-id="487df-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="487df-124">numericComplex</span></span>|<span data-ttu-id="487df-125">4</span><span class="sxs-lookup"><span data-stu-id="487df-125">4</span></span>|<span data-ttu-id="487df-126">Numerische komplexe Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="487df-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="487df-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="487df-127">atLeastAlphabetic</span></span>|<span data-ttu-id="487df-128">5</span><span class="sxs-lookup"><span data-stu-id="487df-128">5</span></span>|<span data-ttu-id="487df-129">Mindestens alphabetische erforderliche Kennwort.</span><span class="sxs-lookup"><span data-stu-id="487df-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="487df-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="487df-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="487df-131">6</span><span class="sxs-lookup"><span data-stu-id="487df-131">6</span></span>|<span data-ttu-id="487df-132">Mindestens Alphanumerisches Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="487df-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="487df-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="487df-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="487df-134">7</span><span class="sxs-lookup"><span data-stu-id="487df-134">7</span></span>|<span data-ttu-id="487df-135">Mindestens alphanumerisch Symbole erforderliche Kennwort.</span><span class="sxs-lookup"><span data-stu-id="487df-135">At least alphanumeric with symbols password required.</span></span>|





