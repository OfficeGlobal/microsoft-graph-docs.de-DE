---
title: SubjectNameFormat Enum-Typ
description: Optionen für Antragstellernamen Format.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 22bbc03da6fd3e48925634704e78ffb22abef3bc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410329"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="ff670-103">SubjectNameFormat Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="ff670-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="ff670-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ff670-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ff670-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff670-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff670-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ff670-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff670-107">Optionen für Antragstellernamen Format.</span><span class="sxs-lookup"><span data-stu-id="ff670-107">Subject Name Format Options.</span></span>

## <a name="members"></a><span data-ttu-id="ff670-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="ff670-108">Members</span></span>
|<span data-ttu-id="ff670-109">Member</span><span class="sxs-lookup"><span data-stu-id="ff670-109">Member</span></span>|<span data-ttu-id="ff670-110">Wert</span><span class="sxs-lookup"><span data-stu-id="ff670-110">Value</span></span>|<span data-ttu-id="ff670-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff670-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff670-112">commonName</span><span class="sxs-lookup"><span data-stu-id="ff670-112">commonName</span></span>|<span data-ttu-id="ff670-113">0</span><span class="sxs-lookup"><span data-stu-id="ff670-113">0</span></span>|<span data-ttu-id="ff670-114">Allgemeiner Name.</span><span class="sxs-lookup"><span data-stu-id="ff670-114">Common name.</span></span>|
|<span data-ttu-id="ff670-115">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="ff670-115">commonNameIncludingEmail</span></span>|<span data-ttu-id="ff670-116">1</span><span class="sxs-lookup"><span data-stu-id="ff670-116">1</span></span>|<span data-ttu-id="ff670-117">Allgemeiner Name, einschließlich E-Mail.</span><span class="sxs-lookup"><span data-stu-id="ff670-117">Common Name Including Email.</span></span>|
|<span data-ttu-id="ff670-118">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="ff670-118">commonNameAsEmail</span></span>|<span data-ttu-id="ff670-119">2</span><span class="sxs-lookup"><span data-stu-id="ff670-119">2</span></span>|<span data-ttu-id="ff670-120">Allgemeiner Name als e-Mail-Nachricht.</span><span class="sxs-lookup"><span data-stu-id="ff670-120">Common Name As Email.</span></span>|
|<span data-ttu-id="ff670-121">custom</span><span class="sxs-lookup"><span data-stu-id="ff670-121">custom</span></span>|<span data-ttu-id="ff670-122">3</span><span class="sxs-lookup"><span data-stu-id="ff670-122">3</span></span>|<span data-ttu-id="ff670-123">Format des benutzerdefinierten Antragstellernamen.</span><span class="sxs-lookup"><span data-stu-id="ff670-123">Custom subject name format.</span></span>|
|<span data-ttu-id="ff670-124">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="ff670-124">commonNameAsIMEI</span></span>|<span data-ttu-id="ff670-125">5</span><span class="sxs-lookup"><span data-stu-id="ff670-125">5</span></span>|<span data-ttu-id="ff670-126">Allgemeiner Name als IMEI.</span><span class="sxs-lookup"><span data-stu-id="ff670-126">Common Name As IMEI.</span></span>|
|<span data-ttu-id="ff670-127">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="ff670-127">commonNameAsSerialNumber</span></span>|<span data-ttu-id="ff670-128">6</span><span class="sxs-lookup"><span data-stu-id="ff670-128">6</span></span>|<span data-ttu-id="ff670-129">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="ff670-129">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="ff670-130">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="ff670-130">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="ff670-131">7</span><span class="sxs-lookup"><span data-stu-id="ff670-131">7</span></span>|<span data-ttu-id="ff670-132">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="ff670-132">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="ff670-133">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="ff670-133">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="ff670-134">8</span><span class="sxs-lookup"><span data-stu-id="ff670-134">8</span></span>|<span data-ttu-id="ff670-135">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="ff670-135">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="ff670-136">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="ff670-136">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="ff670-137">9</span><span class="sxs-lookup"><span data-stu-id="ff670-137">9</span></span>|<span data-ttu-id="ff670-138">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="ff670-138">Common Name As Serial Number.</span></span>|




