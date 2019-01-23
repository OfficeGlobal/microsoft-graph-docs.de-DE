---
title: AndroidDeviceOwnerRequiredPasswordType Enum-Typ
description: Android-Gerät Besitzer Richtlinie erforderliche Kennworttyp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c405cf3a69597994d5539427698baa92cabd3904
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403539"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="578c6-103">AndroidDeviceOwnerRequiredPasswordType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="578c6-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="578c6-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="578c6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="578c6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="578c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="578c6-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="578c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="578c6-107">Android-Gerät Besitzer Richtlinie erforderliche Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="578c6-107">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="578c6-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="578c6-108">Members</span></span>
|<span data-ttu-id="578c6-109">Member</span><span class="sxs-lookup"><span data-stu-id="578c6-109">Member</span></span>|<span data-ttu-id="578c6-110">Wert</span><span class="sxs-lookup"><span data-stu-id="578c6-110">Value</span></span>|<span data-ttu-id="578c6-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="578c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="578c6-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="578c6-112">deviceDefault</span></span>|<span data-ttu-id="578c6-113">0</span><span class="sxs-lookup"><span data-stu-id="578c6-113">0</span></span>|<span data-ttu-id="578c6-114">Gerät Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="578c6-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="578c6-115">erforderlich</span><span class="sxs-lookup"><span data-stu-id="578c6-115">required</span></span>|<span data-ttu-id="578c6-116">1</span><span class="sxs-lookup"><span data-stu-id="578c6-116">1</span></span>|<span data-ttu-id="578c6-117">Es muss ein Kennwort festlegen, jedoch ohne Einschränkungen auf Typ.</span><span class="sxs-lookup"><span data-stu-id="578c6-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="578c6-118">numerische</span><span class="sxs-lookup"><span data-stu-id="578c6-118">numeric</span></span>|<span data-ttu-id="578c6-119">2</span><span class="sxs-lookup"><span data-stu-id="578c6-119">2</span></span>|<span data-ttu-id="578c6-120">AT mindestens numerische.</span><span class="sxs-lookup"><span data-stu-id="578c6-120">At least numeric.</span></span>|
|<span data-ttu-id="578c6-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="578c6-121">numericComplex</span></span>|<span data-ttu-id="578c6-122">3</span><span class="sxs-lookup"><span data-stu-id="578c6-122">3</span></span>|<span data-ttu-id="578c6-123">AT mindestens numerische mit keine wiederholten oder eine geordneten Sequenzen.</span><span class="sxs-lookup"><span data-stu-id="578c6-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="578c6-124">Alphabetische</span><span class="sxs-lookup"><span data-stu-id="578c6-124">alphabetic</span></span>|<span data-ttu-id="578c6-125">4</span><span class="sxs-lookup"><span data-stu-id="578c6-125">4</span></span>|<span data-ttu-id="578c6-126">Mindestens alphabetische Kennwort.</span><span class="sxs-lookup"><span data-stu-id="578c6-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="578c6-127">Alphanumerisch</span><span class="sxs-lookup"><span data-stu-id="578c6-127">alphanumeric</span></span>|<span data-ttu-id="578c6-128">5</span><span class="sxs-lookup"><span data-stu-id="578c6-128">5</span></span>|<span data-ttu-id="578c6-129">Mindestens Alphanumerisches Kennwort</span><span class="sxs-lookup"><span data-stu-id="578c6-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="578c6-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="578c6-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="578c6-131">6</span><span class="sxs-lookup"><span data-stu-id="578c6-131">6</span></span>|<span data-ttu-id="578c6-132">Mindestens alphanumerische durch Geviertstrich.</span><span class="sxs-lookup"><span data-stu-id="578c6-132">At least alphanumeric with symbols.</span></span>|




