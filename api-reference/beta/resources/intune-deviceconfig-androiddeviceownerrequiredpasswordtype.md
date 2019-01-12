---
title: AndroidDeviceOwnerRequiredPasswordType Enum-Typ
description: Android-Gerät Besitzer Richtlinie erforderliche Kennworttyp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b1208de597baff9dd05a48663435a3a928f3dae9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938041"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="b9e1d-103">AndroidDeviceOwnerRequiredPasswordType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="b9e1d-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="b9e1d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b9e1d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9e1d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9e1d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9e1d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b9e1d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9e1d-107">Android-Gerät Besitzer Richtlinie erforderliche Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="b9e1d-107">Android Device Owner policy required password type.</span></span>
## <a name="members"></a><span data-ttu-id="b9e1d-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="b9e1d-108">Members</span></span>
|<span data-ttu-id="b9e1d-109">Element</span><span class="sxs-lookup"><span data-stu-id="b9e1d-109">Member</span></span>|<span data-ttu-id="b9e1d-110">Wert</span><span class="sxs-lookup"><span data-stu-id="b9e1d-110">Value</span></span>|<span data-ttu-id="b9e1d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9e1d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9e1d-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b9e1d-112">deviceDefault</span></span>|<span data-ttu-id="b9e1d-113">0</span><span class="sxs-lookup"><span data-stu-id="b9e1d-113">0</span></span>|<span data-ttu-id="b9e1d-114">Gerät Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="b9e1d-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="b9e1d-115">erforderlich</span><span class="sxs-lookup"><span data-stu-id="b9e1d-115">required</span></span>|<span data-ttu-id="b9e1d-116">1</span><span class="sxs-lookup"><span data-stu-id="b9e1d-116">1</span></span>|<span data-ttu-id="b9e1d-117">Es muss ein Kennwort festlegen, jedoch ohne Einschränkungen auf Typ.</span><span class="sxs-lookup"><span data-stu-id="b9e1d-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="b9e1d-118">numerische</span><span class="sxs-lookup"><span data-stu-id="b9e1d-118">numeric</span></span>|<span data-ttu-id="b9e1d-119">2</span><span class="sxs-lookup"><span data-stu-id="b9e1d-119">2</span></span>|<span data-ttu-id="b9e1d-120">AT mindestens numerische.</span><span class="sxs-lookup"><span data-stu-id="b9e1d-120">At least numeric.</span></span>|
|<span data-ttu-id="b9e1d-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="b9e1d-121">numericComplex</span></span>|<span data-ttu-id="b9e1d-122">3</span><span class="sxs-lookup"><span data-stu-id="b9e1d-122">3</span></span>|<span data-ttu-id="b9e1d-123">AT mindestens numerische mit keine wiederholten oder eine geordneten Sequenzen.</span><span class="sxs-lookup"><span data-stu-id="b9e1d-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="b9e1d-124">Alphabetische</span><span class="sxs-lookup"><span data-stu-id="b9e1d-124">alphabetic</span></span>|<span data-ttu-id="b9e1d-125">4</span><span class="sxs-lookup"><span data-stu-id="b9e1d-125">4</span></span>|<span data-ttu-id="b9e1d-126">Mindestens alphabetische Kennwort.</span><span class="sxs-lookup"><span data-stu-id="b9e1d-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="b9e1d-127">Alphanumerisch</span><span class="sxs-lookup"><span data-stu-id="b9e1d-127">alphanumeric</span></span>|<span data-ttu-id="b9e1d-128">5</span><span class="sxs-lookup"><span data-stu-id="b9e1d-128">5</span></span>|<span data-ttu-id="b9e1d-129">Mindestens Alphanumerisches Kennwort</span><span class="sxs-lookup"><span data-stu-id="b9e1d-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="b9e1d-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="b9e1d-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="b9e1d-131">6</span><span class="sxs-lookup"><span data-stu-id="b9e1d-131">6</span></span>|<span data-ttu-id="b9e1d-132">Mindestens alphanumerische durch Geviertstrich.</span><span class="sxs-lookup"><span data-stu-id="b9e1d-132">At least alphanumeric with symbols.</span></span>|





