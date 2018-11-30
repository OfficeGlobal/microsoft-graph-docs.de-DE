---
title: SubjectNameFormat Enum-Typ
description: Optionen für Antragstellernamen Format.
ms.openlocfilehash: 7299558011c471f02e5c1149da6ac23183faa150
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058309"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="61bf5-103">SubjectNameFormat Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="61bf5-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="61bf5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="61bf5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61bf5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="61bf5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61bf5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="61bf5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61bf5-107">Optionen für Antragstellernamen Format.</span><span class="sxs-lookup"><span data-stu-id="61bf5-107">Subject Name Format Options.</span></span>
## <a name="members"></a><span data-ttu-id="61bf5-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="61bf5-108">Members</span></span>
|<span data-ttu-id="61bf5-109">Element</span><span class="sxs-lookup"><span data-stu-id="61bf5-109">Member</span></span>|<span data-ttu-id="61bf5-110">Wert</span><span class="sxs-lookup"><span data-stu-id="61bf5-110">Value</span></span>|<span data-ttu-id="61bf5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61bf5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61bf5-112">commonName</span><span class="sxs-lookup"><span data-stu-id="61bf5-112">commonName</span></span>|<span data-ttu-id="61bf5-113">0</span><span class="sxs-lookup"><span data-stu-id="61bf5-113">0</span></span>|<span data-ttu-id="61bf5-114">Allgemeiner Name.</span><span class="sxs-lookup"><span data-stu-id="61bf5-114">Common name.</span></span>|
|<span data-ttu-id="61bf5-115">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="61bf5-115">commonNameIncludingEmail</span></span>|<span data-ttu-id="61bf5-116">1</span><span class="sxs-lookup"><span data-stu-id="61bf5-116">1</span></span>|<span data-ttu-id="61bf5-117">Allgemeiner Name, einschließlich E-Mail.</span><span class="sxs-lookup"><span data-stu-id="61bf5-117">Common Name Including Email.</span></span>|
|<span data-ttu-id="61bf5-118">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="61bf5-118">commonNameAsEmail</span></span>|<span data-ttu-id="61bf5-119">2</span><span class="sxs-lookup"><span data-stu-id="61bf5-119">2</span></span>|<span data-ttu-id="61bf5-120">Allgemeiner Name als e-Mail-Nachricht.</span><span class="sxs-lookup"><span data-stu-id="61bf5-120">Common Name As Email.</span></span>|
|<span data-ttu-id="61bf5-121">custom</span><span class="sxs-lookup"><span data-stu-id="61bf5-121">custom</span></span>|<span data-ttu-id="61bf5-122">3</span><span class="sxs-lookup"><span data-stu-id="61bf5-122">3</span></span>|<span data-ttu-id="61bf5-123">Format des benutzerdefinierten Antragstellernamen.</span><span class="sxs-lookup"><span data-stu-id="61bf5-123">Custom subject name format.</span></span>|
|<span data-ttu-id="61bf5-124">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="61bf5-124">commonNameAsIMEI</span></span>|<span data-ttu-id="61bf5-125">5</span><span class="sxs-lookup"><span data-stu-id="61bf5-125">5</span></span>|<span data-ttu-id="61bf5-126">Allgemeiner Name als IMEI.</span><span class="sxs-lookup"><span data-stu-id="61bf5-126">Common Name As IMEI.</span></span>|
|<span data-ttu-id="61bf5-127">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="61bf5-127">commonNameAsSerialNumber</span></span>|<span data-ttu-id="61bf5-128">6</span><span class="sxs-lookup"><span data-stu-id="61bf5-128">6</span></span>|<span data-ttu-id="61bf5-129">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="61bf5-129">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="61bf5-130">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="61bf5-130">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="61bf5-131">7</span><span class="sxs-lookup"><span data-stu-id="61bf5-131">7</span></span>|<span data-ttu-id="61bf5-132">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="61bf5-132">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="61bf5-133">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="61bf5-133">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="61bf5-134">8</span><span class="sxs-lookup"><span data-stu-id="61bf5-134">8</span></span>|<span data-ttu-id="61bf5-135">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="61bf5-135">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="61bf5-136">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="61bf5-136">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="61bf5-137">9</span><span class="sxs-lookup"><span data-stu-id="61bf5-137">9</span></span>|<span data-ttu-id="61bf5-138">Allgemeiner Name als fortlaufende Zahl.</span><span class="sxs-lookup"><span data-stu-id="61bf5-138">Common Name As Serial Number.</span></span>|





