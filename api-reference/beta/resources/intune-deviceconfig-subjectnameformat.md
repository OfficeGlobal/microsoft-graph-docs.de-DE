---
title: SubjectNameFormat Enum-Typ
description: Optionen für Antragstellernamen Format.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 259af745567a0fc5de004f5a804d8bab00355f8f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969590"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="73c97-103">SubjectNameFormat Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="73c97-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="73c97-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="73c97-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73c97-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="73c97-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73c97-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="73c97-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73c97-107">Optionen für Antragstellernamen Format.</span><span class="sxs-lookup"><span data-stu-id="73c97-107">Subject Name Format Options.</span></span>
## <a name="members"></a><span data-ttu-id="73c97-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="73c97-108">Members</span></span>
|<span data-ttu-id="73c97-109">Element</span><span class="sxs-lookup"><span data-stu-id="73c97-109">Member</span></span>|<span data-ttu-id="73c97-110">Wert</span><span class="sxs-lookup"><span data-stu-id="73c97-110">Value</span></span>|<span data-ttu-id="73c97-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73c97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73c97-112">commonName</span><span class="sxs-lookup"><span data-stu-id="73c97-112">commonName</span></span>|<span data-ttu-id="73c97-113">0</span><span class="sxs-lookup"><span data-stu-id="73c97-113">0</span></span>|<span data-ttu-id="73c97-114">Allgemeiner Name.</span><span class="sxs-lookup"><span data-stu-id="73c97-114">Common name.</span></span>|
|<span data-ttu-id="73c97-115">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="73c97-115">commonNameIncludingEmail</span></span>|<span data-ttu-id="73c97-116">1</span><span class="sxs-lookup"><span data-stu-id="73c97-116">1</span></span>|<span data-ttu-id="73c97-117">Allgemeiner Name, einschließlich E-Mail.</span><span class="sxs-lookup"><span data-stu-id="73c97-117">Common Name Including Email.</span></span>|
|<span data-ttu-id="73c97-118">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="73c97-118">commonNameAsEmail</span></span>|<span data-ttu-id="73c97-119">2</span><span class="sxs-lookup"><span data-stu-id="73c97-119">2</span></span>|<span data-ttu-id="73c97-120">Allgemeiner Name als e-Mail-Nachricht.</span><span class="sxs-lookup"><span data-stu-id="73c97-120">Common Name As Email.</span></span>|
|<span data-ttu-id="73c97-121">custom</span><span class="sxs-lookup"><span data-stu-id="73c97-121">custom</span></span>|<span data-ttu-id="73c97-122">3</span><span class="sxs-lookup"><span data-stu-id="73c97-122">3</span></span>|<span data-ttu-id="73c97-123">Format des benutzerdefinierten Antragstellernamen.</span><span class="sxs-lookup"><span data-stu-id="73c97-123">Custom subject name format.</span></span>|
|<span data-ttu-id="73c97-124">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="73c97-124">commonNameAsIMEI</span></span>|<span data-ttu-id="73c97-125">5</span><span class="sxs-lookup"><span data-stu-id="73c97-125">5</span></span>|<span data-ttu-id="73c97-126">Allgemeiner Name als IMEI.</span><span class="sxs-lookup"><span data-stu-id="73c97-126">Common Name As IMEI.</span></span>|
|<span data-ttu-id="73c97-127">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="73c97-127">commonNameAsSerialNumber</span></span>|<span data-ttu-id="73c97-128">6</span><span class="sxs-lookup"><span data-stu-id="73c97-128">6</span></span>|<span data-ttu-id="73c97-129">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="73c97-129">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="73c97-130">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="73c97-130">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="73c97-131">7</span><span class="sxs-lookup"><span data-stu-id="73c97-131">7</span></span>|<span data-ttu-id="73c97-132">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="73c97-132">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="73c97-133">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="73c97-133">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="73c97-134">8</span><span class="sxs-lookup"><span data-stu-id="73c97-134">8</span></span>|<span data-ttu-id="73c97-135">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="73c97-135">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="73c97-136">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="73c97-136">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="73c97-137">9</span><span class="sxs-lookup"><span data-stu-id="73c97-137">9</span></span>|<span data-ttu-id="73c97-138">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="73c97-138">Common Name As Serial Number.</span></span>|





