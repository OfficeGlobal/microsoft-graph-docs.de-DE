---
title: SubjectNameFormat Enum-Typ
description: Optionen für Antragstellernamen Format.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 85a11e8690c360e405df2453229a039ea9f9b1dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821336"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="fec62-103">SubjectNameFormat Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="fec62-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="fec62-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fec62-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fec62-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fec62-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fec62-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fec62-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fec62-107">Optionen für Antragstellernamen Format.</span><span class="sxs-lookup"><span data-stu-id="fec62-107">Subject Name Format Options.</span></span>
## <a name="members"></a><span data-ttu-id="fec62-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="fec62-108">Members</span></span>
|<span data-ttu-id="fec62-109">Element</span><span class="sxs-lookup"><span data-stu-id="fec62-109">Member</span></span>|<span data-ttu-id="fec62-110">Wert</span><span class="sxs-lookup"><span data-stu-id="fec62-110">Value</span></span>|<span data-ttu-id="fec62-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fec62-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fec62-112">commonName</span><span class="sxs-lookup"><span data-stu-id="fec62-112">commonName</span></span>|<span data-ttu-id="fec62-113">0</span><span class="sxs-lookup"><span data-stu-id="fec62-113">0</span></span>|<span data-ttu-id="fec62-114">Allgemeiner Name.</span><span class="sxs-lookup"><span data-stu-id="fec62-114">Common name.</span></span>|
|<span data-ttu-id="fec62-115">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="fec62-115">commonNameIncludingEmail</span></span>|<span data-ttu-id="fec62-116">1</span><span class="sxs-lookup"><span data-stu-id="fec62-116">1</span></span>|<span data-ttu-id="fec62-117">Allgemeiner Name, einschließlich E-Mail.</span><span class="sxs-lookup"><span data-stu-id="fec62-117">Common Name Including Email.</span></span>|
|<span data-ttu-id="fec62-118">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="fec62-118">commonNameAsEmail</span></span>|<span data-ttu-id="fec62-119">2</span><span class="sxs-lookup"><span data-stu-id="fec62-119">2</span></span>|<span data-ttu-id="fec62-120">Allgemeiner Name als e-Mail-Nachricht.</span><span class="sxs-lookup"><span data-stu-id="fec62-120">Common Name As Email.</span></span>|
|<span data-ttu-id="fec62-121">custom</span><span class="sxs-lookup"><span data-stu-id="fec62-121">custom</span></span>|<span data-ttu-id="fec62-122">3</span><span class="sxs-lookup"><span data-stu-id="fec62-122">3</span></span>|<span data-ttu-id="fec62-123">Format des benutzerdefinierten Antragstellernamen.</span><span class="sxs-lookup"><span data-stu-id="fec62-123">Custom subject name format.</span></span>|
|<span data-ttu-id="fec62-124">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="fec62-124">commonNameAsIMEI</span></span>|<span data-ttu-id="fec62-125">5</span><span class="sxs-lookup"><span data-stu-id="fec62-125">5</span></span>|<span data-ttu-id="fec62-126">Allgemeiner Name als IMEI.</span><span class="sxs-lookup"><span data-stu-id="fec62-126">Common Name As IMEI.</span></span>|
|<span data-ttu-id="fec62-127">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="fec62-127">commonNameAsSerialNumber</span></span>|<span data-ttu-id="fec62-128">6</span><span class="sxs-lookup"><span data-stu-id="fec62-128">6</span></span>|<span data-ttu-id="fec62-129">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="fec62-129">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="fec62-130">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="fec62-130">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="fec62-131">7</span><span class="sxs-lookup"><span data-stu-id="fec62-131">7</span></span>|<span data-ttu-id="fec62-132">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="fec62-132">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="fec62-133">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="fec62-133">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="fec62-134">8</span><span class="sxs-lookup"><span data-stu-id="fec62-134">8</span></span>|<span data-ttu-id="fec62-135">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="fec62-135">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="fec62-136">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="fec62-136">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="fec62-137">9</span><span class="sxs-lookup"><span data-stu-id="fec62-137">9</span></span>|<span data-ttu-id="fec62-138">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="fec62-138">Common Name As Serial Number.</span></span>|





