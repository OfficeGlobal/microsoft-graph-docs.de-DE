---
title: androidDeviceOwnerRequiredPasswordType-Enumerationstyp
description: Android-Gerätebesitzer Richtlinie erforderlicher Kennworttyp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 79d71fbabc4597c87c9cee782904334e2f12d7e8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172590"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="1b3f1-103">androidDeviceOwnerRequiredPasswordType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="1b3f1-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="1b3f1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1b3f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b3f1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1b3f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b3f1-106">Android-Gerätebesitzer Richtlinie erforderlicher Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="1b3f1-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="1b3f1-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="1b3f1-107">Members</span></span>
|<span data-ttu-id="1b3f1-108">Element</span><span class="sxs-lookup"><span data-stu-id="1b3f1-108">Member</span></span>|<span data-ttu-id="1b3f1-109">Wert</span><span class="sxs-lookup"><span data-stu-id="1b3f1-109">Value</span></span>|<span data-ttu-id="1b3f1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b3f1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b3f1-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="1b3f1-111">deviceDefault</span></span>|<span data-ttu-id="1b3f1-112">0</span><span class="sxs-lookup"><span data-stu-id="1b3f1-112">0</span></span>|<span data-ttu-id="1b3f1-113">Geräte-Standardwert, keine Absicht.</span><span class="sxs-lookup"><span data-stu-id="1b3f1-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="1b3f1-114">erforderlich</span><span class="sxs-lookup"><span data-stu-id="1b3f1-114">required</span></span>|<span data-ttu-id="1b3f1-115">1</span><span class="sxs-lookup"><span data-stu-id="1b3f1-115">1</span></span>|<span data-ttu-id="1b3f1-116">Es muss ein Kennwort festgelegt sein, es gibt jedoch keine Einschränkungen für den Typ.</span><span class="sxs-lookup"><span data-stu-id="1b3f1-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="1b3f1-117">numerischen</span><span class="sxs-lookup"><span data-stu-id="1b3f1-117">numeric</span></span>|<span data-ttu-id="1b3f1-118">2</span><span class="sxs-lookup"><span data-stu-id="1b3f1-118">2</span></span>|<span data-ttu-id="1b3f1-119">Mindestens numerisch.</span><span class="sxs-lookup"><span data-stu-id="1b3f1-119">At least numeric.</span></span>|
|<span data-ttu-id="1b3f1-120">numericComplex</span><span class="sxs-lookup"><span data-stu-id="1b3f1-120">numericComplex</span></span>|<span data-ttu-id="1b3f1-121">3</span><span class="sxs-lookup"><span data-stu-id="1b3f1-121">3</span></span>|<span data-ttu-id="1b3f1-122">Mindestens eine numerische ohne Wiederhol-oder geordnete Sequenzen.</span><span class="sxs-lookup"><span data-stu-id="1b3f1-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="1b3f1-123">alphabetischer</span><span class="sxs-lookup"><span data-stu-id="1b3f1-123">alphabetic</span></span>|<span data-ttu-id="1b3f1-124">4</span><span class="sxs-lookup"><span data-stu-id="1b3f1-124">4</span></span>|<span data-ttu-id="1b3f1-125">Mindestens ein alphabetisches Kennwort.</span><span class="sxs-lookup"><span data-stu-id="1b3f1-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="1b3f1-126">Alphanumerisch</span><span class="sxs-lookup"><span data-stu-id="1b3f1-126">alphanumeric</span></span>|<span data-ttu-id="1b3f1-127">5</span><span class="sxs-lookup"><span data-stu-id="1b3f1-127">5</span></span>|<span data-ttu-id="1b3f1-128">Mindestens alphanumerisches Kennwort</span><span class="sxs-lookup"><span data-stu-id="1b3f1-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="1b3f1-129">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="1b3f1-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="1b3f1-130">6</span><span class="sxs-lookup"><span data-stu-id="1b3f1-130">6</span></span>|<span data-ttu-id="1b3f1-131">Mindestens alphanumerisch mit Symbolen.</span><span class="sxs-lookup"><span data-stu-id="1b3f1-131">At least alphanumeric with symbols.</span></span>|




