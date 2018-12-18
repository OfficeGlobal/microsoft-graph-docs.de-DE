---
title: SubjectNameFormat Enum-Typ
description: Optionen für Antragstellernamen Format.
author: tfitzmac
ms.openlocfilehash: 61aeddb1e751885c3a0ba39fd5628b71830dded5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307007"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="4122b-103">SubjectNameFormat Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="4122b-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="4122b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4122b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4122b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4122b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4122b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4122b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4122b-107">Optionen für Antragstellernamen Format.</span><span class="sxs-lookup"><span data-stu-id="4122b-107">Subject Name Format Options.</span></span>
## <a name="members"></a><span data-ttu-id="4122b-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="4122b-108">Members</span></span>
|<span data-ttu-id="4122b-109">Member</span><span class="sxs-lookup"><span data-stu-id="4122b-109">Member</span></span>|<span data-ttu-id="4122b-110">Wert</span><span class="sxs-lookup"><span data-stu-id="4122b-110">Value</span></span>|<span data-ttu-id="4122b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4122b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4122b-112">commonName</span><span class="sxs-lookup"><span data-stu-id="4122b-112">commonName</span></span>|<span data-ttu-id="4122b-113">0</span><span class="sxs-lookup"><span data-stu-id="4122b-113">0</span></span>|<span data-ttu-id="4122b-114">Allgemeiner Name.</span><span class="sxs-lookup"><span data-stu-id="4122b-114">Common name.</span></span>|
|<span data-ttu-id="4122b-115">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="4122b-115">commonNameIncludingEmail</span></span>|<span data-ttu-id="4122b-116">1</span><span class="sxs-lookup"><span data-stu-id="4122b-116">1</span></span>|<span data-ttu-id="4122b-117">Allgemeiner Name, einschließlich E-Mail.</span><span class="sxs-lookup"><span data-stu-id="4122b-117">Common Name Including Email.</span></span>|
|<span data-ttu-id="4122b-118">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="4122b-118">commonNameAsEmail</span></span>|<span data-ttu-id="4122b-119">2</span><span class="sxs-lookup"><span data-stu-id="4122b-119">2</span></span>|<span data-ttu-id="4122b-120">Allgemeiner Name als e-Mail-Nachricht.</span><span class="sxs-lookup"><span data-stu-id="4122b-120">Common Name As Email.</span></span>|
|<span data-ttu-id="4122b-121">custom</span><span class="sxs-lookup"><span data-stu-id="4122b-121">custom</span></span>|<span data-ttu-id="4122b-122">3</span><span class="sxs-lookup"><span data-stu-id="4122b-122">3</span></span>|<span data-ttu-id="4122b-123">Format des benutzerdefinierten Antragstellernamen.</span><span class="sxs-lookup"><span data-stu-id="4122b-123">Custom subject name format.</span></span>|
|<span data-ttu-id="4122b-124">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="4122b-124">commonNameAsIMEI</span></span>|<span data-ttu-id="4122b-125">5</span><span class="sxs-lookup"><span data-stu-id="4122b-125">5</span></span>|<span data-ttu-id="4122b-126">Allgemeiner Name als IMEI.</span><span class="sxs-lookup"><span data-stu-id="4122b-126">Common Name As IMEI.</span></span>|
|<span data-ttu-id="4122b-127">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="4122b-127">commonNameAsSerialNumber</span></span>|<span data-ttu-id="4122b-128">6</span><span class="sxs-lookup"><span data-stu-id="4122b-128">6</span></span>|<span data-ttu-id="4122b-129">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="4122b-129">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="4122b-130">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="4122b-130">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="4122b-131">7</span><span class="sxs-lookup"><span data-stu-id="4122b-131">7</span></span>|<span data-ttu-id="4122b-132">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="4122b-132">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="4122b-133">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="4122b-133">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="4122b-134">8</span><span class="sxs-lookup"><span data-stu-id="4122b-134">8</span></span>|<span data-ttu-id="4122b-135">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="4122b-135">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="4122b-136">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="4122b-136">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="4122b-137">9</span><span class="sxs-lookup"><span data-stu-id="4122b-137">9</span></span>|<span data-ttu-id="4122b-138">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="4122b-138">Common Name As Serial Number.</span></span>|





