---
title: AndroidDeviceOwnerRequiredPasswordType Enum-Typ
description: Android-Gerät Besitzer Richtlinie erforderliche Kennworttyp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c53cc67d01886b76a20eef149a59c1d1fef4fc83
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887647"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="5246c-103">AndroidDeviceOwnerRequiredPasswordType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="5246c-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="5246c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5246c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5246c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5246c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5246c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5246c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5246c-107">Android-Gerät Besitzer Richtlinie erforderliche Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="5246c-107">Android Device Owner policy required password type.</span></span>
## <a name="members"></a><span data-ttu-id="5246c-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="5246c-108">Members</span></span>
|<span data-ttu-id="5246c-109">Element</span><span class="sxs-lookup"><span data-stu-id="5246c-109">Member</span></span>|<span data-ttu-id="5246c-110">Wert</span><span class="sxs-lookup"><span data-stu-id="5246c-110">Value</span></span>|<span data-ttu-id="5246c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5246c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5246c-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="5246c-112">deviceDefault</span></span>|<span data-ttu-id="5246c-113">0</span><span class="sxs-lookup"><span data-stu-id="5246c-113">0</span></span>|<span data-ttu-id="5246c-114">Gerät Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="5246c-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="5246c-115">erforderlich</span><span class="sxs-lookup"><span data-stu-id="5246c-115">required</span></span>|<span data-ttu-id="5246c-116">1</span><span class="sxs-lookup"><span data-stu-id="5246c-116">1</span></span>|<span data-ttu-id="5246c-117">Es muss ein Kennwort festlegen, jedoch ohne Einschränkungen auf Typ.</span><span class="sxs-lookup"><span data-stu-id="5246c-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="5246c-118">numerische</span><span class="sxs-lookup"><span data-stu-id="5246c-118">numeric</span></span>|<span data-ttu-id="5246c-119">2</span><span class="sxs-lookup"><span data-stu-id="5246c-119">2</span></span>|<span data-ttu-id="5246c-120">AT mindestens numerische.</span><span class="sxs-lookup"><span data-stu-id="5246c-120">At least numeric.</span></span>|
|<span data-ttu-id="5246c-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="5246c-121">numericComplex</span></span>|<span data-ttu-id="5246c-122">3</span><span class="sxs-lookup"><span data-stu-id="5246c-122">3</span></span>|<span data-ttu-id="5246c-123">AT mindestens numerische mit keine wiederholten oder eine geordneten Sequenzen.</span><span class="sxs-lookup"><span data-stu-id="5246c-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="5246c-124">Alphabetische</span><span class="sxs-lookup"><span data-stu-id="5246c-124">alphabetic</span></span>|<span data-ttu-id="5246c-125">4</span><span class="sxs-lookup"><span data-stu-id="5246c-125">4</span></span>|<span data-ttu-id="5246c-126">Mindestens alphabetische Kennwort.</span><span class="sxs-lookup"><span data-stu-id="5246c-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="5246c-127">Alphanumerisch</span><span class="sxs-lookup"><span data-stu-id="5246c-127">alphanumeric</span></span>|<span data-ttu-id="5246c-128">5</span><span class="sxs-lookup"><span data-stu-id="5246c-128">5</span></span>|<span data-ttu-id="5246c-129">Mindestens Alphanumerisches Kennwort</span><span class="sxs-lookup"><span data-stu-id="5246c-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="5246c-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="5246c-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="5246c-131">6</span><span class="sxs-lookup"><span data-stu-id="5246c-131">6</span></span>|<span data-ttu-id="5246c-132">Mindestens alphanumerische durch Geviertstrich.</span><span class="sxs-lookup"><span data-stu-id="5246c-132">At least alphanumeric with symbols.</span></span>|





