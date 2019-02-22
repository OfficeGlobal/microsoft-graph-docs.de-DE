---
title: subjectNameFormat-Enumerationstyp
description: Format Optionen für den AntragsTellernamen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f12068576ff78d74f2e1b6119a2030ff7835a7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158555"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="456f8-103">subjectNameFormat-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="456f8-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="456f8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="456f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="456f8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="456f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="456f8-106">Format Optionen für den AntragsTellernamen.</span><span class="sxs-lookup"><span data-stu-id="456f8-106">Subject Name Format Options.</span></span>

## <a name="members"></a><span data-ttu-id="456f8-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="456f8-107">Members</span></span>
|<span data-ttu-id="456f8-108">Element</span><span class="sxs-lookup"><span data-stu-id="456f8-108">Member</span></span>|<span data-ttu-id="456f8-109">Wert</span><span class="sxs-lookup"><span data-stu-id="456f8-109">Value</span></span>|<span data-ttu-id="456f8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="456f8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="456f8-111">commonName</span><span class="sxs-lookup"><span data-stu-id="456f8-111">commonName</span></span>|<span data-ttu-id="456f8-112">0</span><span class="sxs-lookup"><span data-stu-id="456f8-112">0</span></span>|<span data-ttu-id="456f8-113">Allgemeiner Name.</span><span class="sxs-lookup"><span data-stu-id="456f8-113">Common name.</span></span>|
|<span data-ttu-id="456f8-114">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="456f8-114">commonNameIncludingEmail</span></span>|<span data-ttu-id="456f8-115">1</span><span class="sxs-lookup"><span data-stu-id="456f8-115">1</span></span>|<span data-ttu-id="456f8-116">Allgemeiner Name, einschließlich E-Mail.</span><span class="sxs-lookup"><span data-stu-id="456f8-116">Common Name Including Email.</span></span>|
|<span data-ttu-id="456f8-117">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="456f8-117">commonNameAsEmail</span></span>|<span data-ttu-id="456f8-118">2</span><span class="sxs-lookup"><span data-stu-id="456f8-118">2</span></span>|<span data-ttu-id="456f8-119">Allgemeiner Name als E-Mail.</span><span class="sxs-lookup"><span data-stu-id="456f8-119">Common Name As Email.</span></span>|
|<span data-ttu-id="456f8-120">custom</span><span class="sxs-lookup"><span data-stu-id="456f8-120">custom</span></span>|<span data-ttu-id="456f8-121">3</span><span class="sxs-lookup"><span data-stu-id="456f8-121">3</span></span>|<span data-ttu-id="456f8-122">Format für benutzerdefinierte Antragstellernamen.</span><span class="sxs-lookup"><span data-stu-id="456f8-122">Custom subject name format.</span></span>|
|<span data-ttu-id="456f8-123">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="456f8-123">commonNameAsIMEI</span></span>|<span data-ttu-id="456f8-124">5</span><span class="sxs-lookup"><span data-stu-id="456f8-124">5</span></span>|<span data-ttu-id="456f8-125">Allgemeiner Name als IMEI.</span><span class="sxs-lookup"><span data-stu-id="456f8-125">Common Name As IMEI.</span></span>|
|<span data-ttu-id="456f8-126">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="456f8-126">commonNameAsSerialNumber</span></span>|<span data-ttu-id="456f8-127">6</span><span class="sxs-lookup"><span data-stu-id="456f8-127">6</span></span>|<span data-ttu-id="456f8-128">Allgemeiner Name als Seriennummer.</span><span class="sxs-lookup"><span data-stu-id="456f8-128">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="456f8-129">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="456f8-129">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="456f8-130">7</span><span class="sxs-lookup"><span data-stu-id="456f8-130">7</span></span>|<span data-ttu-id="456f8-131">Allgemeiner Name als Seriennummer.</span><span class="sxs-lookup"><span data-stu-id="456f8-131">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="456f8-132">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="456f8-132">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="456f8-133">8</span><span class="sxs-lookup"><span data-stu-id="456f8-133">8</span></span>|<span data-ttu-id="456f8-134">Allgemeiner Name als Seriennummer.</span><span class="sxs-lookup"><span data-stu-id="456f8-134">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="456f8-135">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="456f8-135">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="456f8-136">9</span><span class="sxs-lookup"><span data-stu-id="456f8-136">9</span></span>|<span data-ttu-id="456f8-137">Allgemeiner Name als Seriennummer.</span><span class="sxs-lookup"><span data-stu-id="456f8-137">Common Name As Serial Number.</span></span>|




